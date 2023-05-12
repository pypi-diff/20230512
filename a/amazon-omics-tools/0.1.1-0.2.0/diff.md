# Comparing `tmp/amazon-omics-tools-0.1.1.tar.gz` & `tmp/amazon_omics_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-omics-tools-0.1.1.tar", max compression
+gzip compressed data, was "amazon_omics_tools-0.2.0.tar", max compression
```

## Comparing `amazon-omics-tools-0.1.1.tar` & `amazon_omics_tools-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0    10142 2022-11-02 23:00:51.698645 amazon-omics-tools-0.1.1/LICENSE
--rw-r--r--   0        0        0     2936 2022-11-29 22:16:43.936802 amazon-omics-tools-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-11-11 00:23:59.267573 amazon-omics-tools-0.1.1/omics/__init__.py
--rw-r--r--   0        0        0     3710 2022-11-25 03:42:22.219680 amazon-omics-tools-0.1.1/omics/transfer/__init__.py
--rw-r--r--   0        0        0     3585 2022-11-25 03:42:22.220186 amazon-omics-tools-0.1.1/omics/transfer/config.py
--rw-r--r--   0        0        0     8855 2022-11-25 03:42:22.220605 amazon-omics-tools-0.1.1/omics/transfer/download.py
--rw-r--r--   0        0        0    21145 2022-11-29 20:27:23.596268 amazon-omics-tools-0.1.1/omics/transfer/manager.py
--rw-r--r--   0        0        0     1246 2022-11-29 22:16:43.938016 amazon-omics-tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 amazon-omics-tools-0.1.1/setup.py
--rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 amazon-omics-tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-05-11 19:57:24.703573 amazon_omics_tools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5724 2023-05-11 22:18:22.000000 amazon_omics_tools-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 17:44:30.000000 amazon_omics_tools-0.2.0/omics/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:16:56.000000 amazon_omics_tools-0.2.0/omics/common/__init__.py
+-rw-r--r--   0        0        0     1819 2023-05-11 22:18:22.000000 amazon_omics_tools-0.2.0/omics/common/omics_file_types.py
+-rw-r--r--   0        0        0     3405 2023-05-11 22:18:22.000000 amazon_omics_tools-0.2.0/omics/transfer/__init__.py
+-rw-r--r--   0        0        0     3853 2023-05-11 22:18:22.000000 amazon_omics_tools-0.2.0/omics/transfer/config.py
+-rw-r--r--   0        0        0     8894 2023-05-11 22:18:22.000000 amazon_omics_tools-0.2.0/omics/transfer/download.py
+-rw-r--r--   0        0        0    25861 2023-05-11 22:18:22.000000 amazon_omics_tools-0.2.0/omics/transfer/manager.py
+-rw-r--r--   0        0        0    11149 2023-05-11 22:18:22.000000 amazon_omics_tools-0.2.0/omics/transfer/read_set_upload.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:16:56.000000 amazon_omics_tools-0.2.0/omics/uriparse/__init__.py
+-rw-r--r--   0        0        0     2509 2023-03-24 16:16:56.000000 amazon_omics_tools-0.2.0/omics/uriparse/uri_parse.py
+-rw-r--r--   0        0        0     1259 2023-05-12 15:51:44.490089 amazon_omics_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6728 1970-01-01 00:00:00.000000 amazon_omics_tools-0.2.0/setup.py
+-rw-r--r--   0        0        0     6489 1970-01-01 00:00:00.000000 amazon_omics_tools-0.2.0/PKG-INFO
```

### Comparing `amazon-omics-tools-0.1.1/LICENSE` & `amazon_omics_tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-omics-tools-0.1.1/omics/transfer/__init__.py` & `amazon_omics_tools-0.2.0/omics/transfer/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,121 +1,100 @@
-from enum import Enum
-from typing import IO, Any, List, Type, Union
+from typing import IO, Any, Dict, List, Optional, Union
 
 from s3transfer.futures import TransferFuture
 from s3transfer.subscribers import BaseSubscriber
 
+from omics.common.omics_file_types import OmicsFileType, ReadSetFileType
+
 
 class OmicsTransferSubscriber(BaseSubscriber):
     """Base class for subscribers of Omics data transfer."""
 
 
 class OmicsTransferFuture(TransferFuture):
     """Future for getting the result of Omics data transfer."""
 
 
-class ExtendedEnum(Enum):
-    """Enum subclass that includes helper methods."""
-
-    @classmethod
-    def list(cls: Type[Enum]) -> List[str]:
-        """Return the list of allowed values in an Enum."""
-        return list(map(lambda c: c.value, cls))  # type: ignore
-
-    @classmethod
-    def from_object(cls: Type[Enum], object: Any) -> Enum:
-        """Convert an object to the Enum type if possible.
-
-        Since Python allows strings to be passed as parameters even when an Enum
-        type is specified, this method converts a string to an enum if it
-        matches one of the allowed values.
-
-        Args:
-            object: the object to convert to an Enum.
-        """
-        if type(object) == cls:
-            return object
-        if type(object) == str:
-            for enum in cls:
-                if object.upper() == enum.value:
-                    return enum
-            valid_values = ", ".join(cls.list())
-            raise AttributeError(f"{cls.__name__} must be one of {valid_values}")
-
-        raise AttributeError(f"Unsupported type for {cls.__name__}: {type(object)}")
-
-
-class ReadSetFileName(ExtendedEnum):
-    """Available read set file names."""
-
-    SOURCE1 = "SOURCE1"
-    SOURCE2 = "SOURCE2"
-    INDEX = "INDEX"
-
-
-class ReferenceFileName(ExtendedEnum):
-    """Available reference file names."""
-
-    SOURCE = "SOURCE"
-    INDEX = "INDEX"
-
-
-class FileTransferDirection(ExtendedEnum):
-    """Available transfer directions (UP = upload, DOWN = download)."""
-
-    UP = "UP"
-    DOWN = "DOWN"
-
-
-class OmicsFileType(ExtendedEnum):
-    """Available file types."""
-
-    READ_SET = "READ_SET"
-    REFERENCE = "REFERENCE"
-
-
-class FileTransfer:
-    """Details of an Omics file transfer."""
+class FileDownload:
+    """Details of an Omics file download."""
 
     def __init__(
         self,
         store_id: str,
         file_set_id: str,
         filename: str,
         fileobj: Union[IO[Any], str],
         omics_file_type: OmicsFileType,
-        direction: FileTransferDirection = FileTransferDirection.DOWN,
         subscribers: List[BaseSubscriber] = None,
     ):
         """Details of a file download.
 
         Args:
             store_id: the ID of the data store (either Reference Store or Sequence Store).
 
             file_set_id: Reference ID or Read Set ID.
 
-            filename: the name of the file when it it stored on the server.
+            filename: the name of the file when it is stored on the server.
 
             fileobj: The name of a file or IO object to transfer data to.
 
             omics_file_type: the type of Omics file being transferred.
 
-            orig_filename: The original name of the data file (ex: "NA12878.cram")
-
-            direction: currently only DOWN (download) is supported.
-
             subscribers: The list of subscribers to be invoked in the
                 order provided based on the event emit during the process of
                 the transfer request.
         """
-        self.direction = direction
         self.omics_file_type = omics_file_type
         self.store_id = store_id
         self.file_set_id = file_set_id
         self.filename = filename
         self.fileobj = fileobj
         self.subscribers = [] if subscribers is None else subscribers
 
         if filename is None:
             raise AttributeError("filename cannot be None")
-        if direction != FileTransferDirection.DOWN:
-            raise AttributeError("Only download is currently supported (direction = DOWN)")
+
+
+class ReadSetUpload:
+    """Details of an Omics read set upload."""
+
+    def __init__(
+        self,
+        store_id: str,
+        file_type: ReadSetFileType,
+        name: str,
+        subject_id: str,
+        sample_id: str,
+        reference_arn: str,
+        fileobj: Union[IO[Any], str],
+        generated_from: Optional[str] = None,
+        description: Optional[str] = None,
+        tags: Optional[Dict[str, str]] = None,
+        subscribers: Optional[List[BaseSubscriber]] = None,
+    ):
+        """Details of a read set upload.
+
+        :param store_id: The store ID
+        :param file_type: The read set file type being uploaded
+        :param name: The name of the read set
+        :param subject_id: The subject for the read set
+        :param sample_id: The sample for the read set
+        :param reference_arn: The reference ARN
+        :param fileobj: The file being uploaded
+        :param generated_from: Where the file was generated from
+        :param description: The description of the read set
+        :param tags: Tags to add to the read set
+        :param subscribers: The list of subscribers to be invoked in the
+                order provided based on the event emit during the process of
+                the transfer request.
+        """
+        self.store_id = store_id
+        self.file_type = file_type
+        self.name = name
+        self.subject_id = subject_id
+        self.sample_id = sample_id
+        self.reference_arn = reference_arn
+        self.fileobj = fileobj
+        self.generated_from = generated_from
+        self.description = description
+        self.tags = tags
+        self.subscribers = [] if subscribers is None else subscribers
```

### Comparing `amazon-omics-tools-0.1.1/omics/transfer/config.py` & `amazon_omics_tools-0.2.0/omics/transfer/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         max_request_concurrency: int = 10,
         max_submission_concurrency: int = 5,
         max_request_queue_size: int = 1000,
         max_submission_queue_size: int = 1000,
         max_io_queue_size: int = 1000,
         io_chunksize: int = 256 * KB,
         num_download_attempts: int = 5,
+        max_bandwidth: int = None,
     ):
         """Create a Transfer Manager configuration.
 
         Args:
             use_threads: If True, threads will be used.
                 If False, no threads will be used in performing transfers;
                 all logic will be run in the main thread.
@@ -53,24 +54,29 @@
                 that these retries account for errors that occur when streaming
                 down the data from Omics (i.e. socket errors and read timeouts that
                 occur after receiving an OK response from Omics).
                 Other retryable exceptions such as throttling errors and 5xx errors
                 are already retried by botocore (this default is 5). The
                 ``num_download_attempts`` does not take into account the
                 number of exceptions retried by botocore.
+
+            max_bandwidth: The maximum bandwidth that will be consumed
+                in uploading and downloading file content. The value is in terms of
+                bytes per second.
         """
         self.use_threads = use_threads
         self.directory = directory
         self.max_request_concurrency = max_request_concurrency
         self.max_submission_concurrency = max_submission_concurrency
         self.max_request_queue_size = max_request_queue_size
         self.max_submission_queue_size = max_submission_queue_size
         self.max_io_queue_size = max_io_queue_size
         self.io_chunksize = io_chunksize
         self.num_download_attempts = num_download_attempts
+        self.max_bandwidth = max_bandwidth
         self._validate_attrs_are_nonzero()
 
     def _validate_attrs_are_nonzero(self) -> None:
         for attr, attr_val in self.__dict__.items():
             if attr_val is not None and (type(attr_val) == int) and attr_val <= 0:
                 raise ValueError(
                     "Provided parameter %s of value %s must be greater than "
```

### Comparing `amazon-omics-tools-0.1.1/omics/transfer/download.py` & `amazon_omics_tools-0.2.0/omics/transfer/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     CountCallbackInvoker,
     FunctionContainer,
     StreamReaderProgress,
     get_callbacks,
     invoke_progress_callbacks,
 )
 
-from omics.transfer import FileTransfer, OmicsFileType
+from omics.common.omics_file_types import OmicsFileType
+from omics.transfer import FileDownload
 from omics.transfer.config import TransferConfig
 
 logger = logging.getLogger(__name__)
 
 # In python 3, all the socket related errors are in a newly created ConnectionError.
 SOCKET_ERROR = ConnectionError
 RETRYABLE_DOWNLOAD_ERRORS = (
@@ -51,22 +52,22 @@
     ) -> None:
         # Get the needed progress callbacks for the task
         progress_callbacks = get_callbacks(transfer_future, "progress")
 
         # Get a handle to the file that will be used for writing downloaded contents
         fileobj = download_manager.get_fileobj_for_io_writes(transfer_future)
 
-        transfer_args: FileTransfer = transfer_future.meta.call_args  # type: ignore
+        transfer_args: FileDownload = transfer_future.meta.call_args  # type: ignore
 
         if transfer_args.omics_file_type == OmicsFileType.REFERENCE:
             metadata_response = client.get_reference_metadata(
                 referenceStoreId=transfer_args.store_id, id=transfer_args.file_set_id
             )
             metadata_files = metadata_response["files"]
-        elif transfer_args.omics_file_type == OmicsFileType.READ_SET:
+        elif transfer_args.omics_file_type == OmicsFileType.READSET:
             metadata_response = client.get_read_set_metadata(
                 sequenceStoreId=transfer_args.store_id, id=transfer_args.file_set_id
             )  # type: ignore
             metadata_files = metadata_response["files"]
         else:
             raise AttributeError(f"Unexpected Omics file type: {transfer_args.omics_file_type}")
 
@@ -144,15 +145,15 @@
                 if omics_file_type == OmicsFileType.REFERENCE:
                     response = client.get_reference(
                         referenceStoreId=store_id,
                         id=file_set_id,
                         partNumber=part_number,
                         file=file,
                     )
-                elif omics_file_type == OmicsFileType.READ_SET:
+                elif omics_file_type == OmicsFileType.READSET:
                     response = client.get_read_set(
                         sequenceStoreId=store_id,
                         id=file_set_id,
                         partNumber=part_number,
                         file=file,
                     )
                 else:
```

### Comparing `amazon-omics-tools-0.1.1/omics/transfer/manager.py` & `amazon_omics_tools-0.2.0/omics/transfer/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,49 @@
+import logging
 import os
 import re
 from concurrent.futures import CancelledError
-from typing import IO, Any, List, Type, Union
+from typing import IO, Any, Dict, List, Optional, Type, Union
 
 from mypy_boto3_omics.client import OmicsClient
+from s3transfer.bandwidth import BandwidthLimiter, LeakyBucket
 from s3transfer.download import (
     DownloadNonSeekableOutputManager,
     DownloadOutputManager,
     DownloadSeekableOutputManager,
 )
 from s3transfer.exceptions import FatalError
 from s3transfer.futures import (
     BoundedExecutor,
     NonThreadedExecutor,
     TransferCoordinator,
+    TransferFuture,
     TransferMeta,
 )
 from s3transfer.manager import TransferCoordinatorController
 from s3transfer.utils import OSUtils, get_callbacks
 
-from omics.transfer import (
-    FileTransfer,
-    FileTransferDirection,
+from omics.common.omics_file_types import (
     OmicsFileType,
-    OmicsTransferFuture,
-    OmicsTransferSubscriber,
     ReadSetFileName,
+    ReadSetFileType,
     ReferenceFileName,
 )
+from omics.transfer import (
+    FileDownload,
+    OmicsTransferFuture,
+    OmicsTransferSubscriber,
+    ReadSetUpload,
+)
 from omics.transfer.config import TransferConfig
 from omics.transfer.download import (
     DownloadSubmissionTask,
     OmicsDownloadFilenameOutputManager,
 )
+from omics.transfer.read_set_upload import ReadSetUploadSubmissionTask
 
 DONE_CALLBACK_TYPE: str = "done"
 
 # The only supported file type for references is FASTA.
 REFERENCE_FILE_TYPE: str = "FASTA"
 
 # Map of file type to data file extension.
@@ -50,14 +57,16 @@
 # Map of file type to index file extension.
 FILE_TYPE_INDEX_EXTENSION_MAP: dict[str, str] = {
     "FASTA": "fasta.fai",
     "BAM": "bam.bai",
     "CRAM": "cram.crai",
 }
 
+logger = logging.getLogger(__name__)
+
 
 class TransferManager:
     """Omics data transfer manager which uses multiple threads for parallel processing."""
 
     def __init__(
         self,
         client: OmicsClient,
@@ -102,14 +111,21 @@
         # downloads for all files.
         self._io_executor = BoundedExecutor(
             max_size=self._config.max_io_queue_size,
             max_num_threads=1,
             executor_cls=executor_cls,
         )
 
+        # The component responsible for limiting bandwidth usage if it is configured.
+        self._bandwidth_limiter = None
+        if self._config.max_bandwidth is not None:
+            logger.debug(f"Setting max_bandwidth to {self._config.max_bandwidth}")
+            leaky_bucket = LeakyBucket(self._config.max_bandwidth)
+            self._bandwidth_limiter = BandwidthLimiter(leaky_bucket)
+
     def download_reference(
         self,
         reference_store_id: str,
         reference_id: str,
         directory: str = None,
         subscribers: List[OmicsTransferSubscriber] = [],
         wait: bool = True,
@@ -320,47 +336,138 @@
                     server_filename,
                     read_set_metadata["fileType"],
                     add_source_counter,
                 ),
             )
 
         return self._download_file(
-            OmicsFileType.READ_SET,
+            OmicsFileType.READSET,
             sequence_store_id,
             read_set_id,
             server_filename_enum.value,
             client_fileobj,
             subscribers,
             wait,
         )
 
+    def upload_read_set(
+        self,
+        fileobjs: Union[IO[Any], str, List[Union[IO[Any], str]]],
+        sequence_store_id: str,
+        file_type: ReadSetFileType,
+        name: str,
+        subject_id: str,
+        sample_id: str,
+        reference_arn: str,
+        generated_from: Optional[str] = None,
+        description: Optional[str] = None,
+        tags: Optional[Dict[str, str]] = None,
+        subscribers: Optional[List[OmicsTransferSubscriber]] = None,
+        wait: bool = True,
+    ) -> Union[TransferFuture, str]:
+        """Upload files and create a read set.
+
+        :param fileobjs: One or two file-like objects to be uploaded as a read set
+        :param sequence_store_id: ID of the Omics sequence store.
+        :param file_type: The type of file being uploaded.
+        :param name: The name of the read set.
+        :param subject_id: The subject ID for the read set.
+        :param sample_id: The sample ID for the read set.
+        :param reference_arn: The reference ARN.
+        :param generated_from: Where the file was generated from.
+        :param description: The description of the read set.
+        :param tags: Tags to assign to the read set.
+        :param subscribers: One or more subscribers for receiving transfer events.
+        :param wait: True = block until all files have been uploaded (default).
+            False = return a futures for controlling how to wait.
+        :return: The ID of the created read set or a future returning it.
+        """
+        # Always treat fileobjs as a list even if we only have a single file
+        fileobjs = fileobjs if type(fileobjs) is list else [fileobjs]  # type: ignore
+
+        if len(fileobjs) > 2:
+            raise AttributeError("at most two files can be uploaded to a read set")
+
+        if len(fileobjs) > 1 and file_type is not ReadSetFileType.FASTQ:
+            raise AttributeError("paired end read files only supported for FASTQ")
+
+        transfer_coordinator = self._get_future_coordinator()
+        transfer_futures = []
+        for fileobj in fileobjs:
+            upload_args = ReadSetUpload(
+                store_id=sequence_store_id,
+                file_type=file_type,
+                name=name,
+                subject_id=subject_id,
+                sample_id=sample_id,
+                reference_arn=reference_arn,
+                fileobj=fileobj,
+                generated_from=generated_from,
+                description=description,
+                tags=tags,
+                subscribers=subscribers,
+            )
+
+            transfer_meta = TransferMeta(upload_args, transfer_coordinator.transfer_id)
+            transfer_futures.append(OmicsTransferFuture(transfer_meta, transfer_coordinator))
+
+        transfer_future = transfer_futures[0]
+        paired_transfer_future = None if len(transfer_futures) < 2 else transfer_futures[1]
+
+        # Add any provided done callbacks to the first created transfer future
+        # to be invoked on the entire upload being complete.
+        for callback in get_callbacks(transfer_future, DONE_CALLBACK_TYPE):
+            transfer_coordinator.add_done_callback(callback)
+
+        # Return the upload task so that users can await the read set ID it creates
+        self._submission_executor.submit(
+            ReadSetUploadSubmissionTask(
+                transfer_coordinator=transfer_coordinator,
+                main_kwargs={
+                    "client": self._client,
+                    "osutil": self._osutil,
+                    "request_executor": self._request_executor,
+                    "transfer_future": transfer_future,
+                    "paired_transfer_future": paired_transfer_future,
+                    "bandwidth_limiter": self._bandwidth_limiter,
+                },
+            )
+        )
+
+        return transfer_future if not wait else transfer_future.result()
+
+    def _get_future_coordinator(self) -> TransferCoordinator:
+        transfer_id = self._get_next_transfer_id()
+        # Creates a new transfer future along with its components
+        transfer_coordinator = TransferCoordinator(transfer_id=transfer_id)
+        # Track the transfer coordinator for transfers to manage.
+        self._coordinator_controller.add_transfer_coordinator(transfer_coordinator)
+        # Also make sure that the transfer coordinator is removed once
+        # the transfer completes so it does not stick around in memory.
+        transfer_coordinator.add_done_callback(
+            self._coordinator_controller.remove_transfer_coordinator,
+            transfer_coordinator,
+        )
+        return transfer_coordinator
+
     def _download_file(
         self,
         omics_file_type: OmicsFileType,
         store_id: str,
         file_set_id: str,
         server_filename: str,
         client_fileobj: Union[IO[Any], str],
         subscribers: List[OmicsTransferSubscriber] = [],
         wait: bool = False,
     ) -> OmicsTransferFuture:
         """Private helper method for downloading a file."""
-        transfer_id = self._get_next_transfer_id()
-        transfer_coordinator = TransferCoordinator(transfer_id=transfer_id)
-
-        # Also make sure that the transfer coordinator is removed once
-        # the transfer completes so it does not stick around in memory.
-        transfer_coordinator.add_done_callback(
-            self._coordinator_controller.remove_transfer_coordinator,
-            transfer_coordinator,
-        )
-
         if client_fileobj is None:
             raise ValueError("client_fileobj parameter is required")
 
+        transfer_coordinator = self._get_future_coordinator()
         if OmicsDownloadFilenameOutputManager.is_compatible(client_fileobj, self._osutil):
             download_manager: DownloadOutputManager = OmicsDownloadFilenameOutputManager(
                 self._osutil, transfer_coordinator, self._io_executor
             )
         elif DownloadSeekableOutputManager.is_compatible(client_fileobj, self._osutil):
             download_manager = DownloadSeekableOutputManager(
                 self._osutil, transfer_coordinator, self._io_executor
@@ -368,35 +475,30 @@
         elif DownloadNonSeekableOutputManager.is_compatible(client_fileobj, self._osutil):
             download_manager = DownloadNonSeekableOutputManager(
                 self._osutil, transfer_coordinator, self._io_executor
             )
         else:
             raise ValueError(f"The client_fileobj (type: {type(client_fileobj)}) is not supported")
 
-        file_transfer = FileTransfer(
+        file_transfer = FileDownload(
             store_id=store_id,
             file_set_id=file_set_id,
             filename=server_filename,
             fileobj=client_fileobj,
             subscribers=subscribers,
-            direction=FileTransferDirection.DOWN,
             omics_file_type=omics_file_type,
         )
-
-        transfer_meta = TransferMeta(file_transfer, transfer_id=transfer_id)
+        transfer_meta = TransferMeta(file_transfer, transfer_coordinator.transfer_id)
         transfer_future = OmicsTransferFuture(transfer_meta, transfer_coordinator)
 
         # Add any provided done callbacks to the created transfer future
         # to be invoked on the transfer future being complete.
         for callback in get_callbacks(transfer_future, DONE_CALLBACK_TYPE):
             transfer_coordinator.add_done_callback(callback)
 
-        # Track the transfer coordinator for transfers to manage.
-        self._coordinator_controller.add_transfer_coordinator(transfer_coordinator)
-
         main_kwargs = {
             "client": self._client,
             "config": self._config,
             "request_executor": self._request_executor,
             "transfer_future": transfer_future,
             "download_manager": download_manager,
             "io_executor": self._io_executor,
@@ -424,15 +526,15 @@
         return self
 
     def __exit__(self, exc_type: Type[BaseException], exc_value: BaseException, *args: Any) -> None:
         """Clean up when a 'with' block is complete."""
         cancel = False
         cancel_msg = ""
         cancel_exc_type: Type[BaseException] = FatalError
-        # If a exception was raised in the context handler, signal to cancel
+        # If an exception was raised in the context handler, signal to cancel
         # all of the in progress futures in the shutdown.
         if exc_type:
             cancel = True
             cancel_msg = str(exc_value)
             if not cancel_msg:
                 cancel_msg = repr(exc_value)
             # If it was a KeyboardInterrupt, the cancellation was initiated
```

### Comparing `amazon-omics-tools-0.1.1/pyproject.toml` & `amazon_omics_tools-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "amazon-omics-tools"
-version = "0.1.1"
+version = "0.2.0"
 license = "Apache-2.0"
 description = "Tools for working with the Amazon Omics Service"
 repository = "https://github.com/awslabs/amazon-omics-tools"
 authors = ["Amazon Web Services"]
 readme = "README.md"
 packages = [{ include = "omics" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 s3transfer = "^0.6.0"
-boto3 = "^1.26.19"
-mypy-boto3-omics = "^1.26.19"
+boto3 = "^1.26.133"
+mypy-boto3-omics = "^1.26.133"
+botocore-stubs = "^1.29.130"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 pytest = "^7.1.3"
 mypy = "^0.971"
 flake8 = "^5.0.4"
 flake8-docstrings = "^1.6.0"
 isort = "^5.10.1"
 pytest-cov = "^4.0.0"
 pytest-rerunfailures = "^10.2"
 types-s3transfer = "^0.6.0.post4"
 types-setuptools = "^65.4.0.0"
-bandit = "^1.7.4"
 pip-audit = "^2.4.4"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 multi_line_output = 3
```

