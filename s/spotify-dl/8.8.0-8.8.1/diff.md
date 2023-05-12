# Comparing `tmp/spotify_dl-8.8.0.tar.gz` & `tmp/spotify_dl-8.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_dl-8.8.0.tar", last modified: Wed May 10 08:18:09 2023, max compression
+gzip compressed data, was "spotify_dl-8.8.1.tar", last modified: Fri May 12 15:34:10 2023, max compression
```

## Comparing `spotify_dl-8.8.0.tar` & `spotify_dl-8.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/spotify_dl/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/spotify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6709 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/spotify_dl.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/spotify_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/spotify_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/spotify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6663 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/spotify_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-05-12 15:33:58.000000 spotify_dl-8.8.1/spotify_dl/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:34:10.139443 spotify_dl-8.8.1/spotify_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 15:34:10.000000 spotify_dl-8.8.1/spotify_dl.egg-info/top_level.txt
```

### Comparing `spotify_dl-8.8.0/LICENSE` & `spotify_dl-8.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.0/PKG-INFO` & `spotify_dl-8.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_dl
-Version: 8.8.0
+Version: 8.8.1
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spotify_dl-8.8.0/README.md` & `spotify_dl-8.8.1/README.md`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.0/setup.py` & `spotify_dl-8.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.0/spotify_dl/scaffold.py` & `spotify_dl-8.8.1/spotify_dl/scaffold.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.0/spotify_dl/spotify.py` & `spotify_dl-8.8.1/spotify_dl/spotify.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.8.0/spotify_dl/spotify_dl.py` & `spotify_dl-8.8.1/spotify_dl/spotify_dl.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 from spotify_dl.spotify import (
     fetch_tracks,
     parse_spotify_url,
     validate_spotify_urls,
     get_item_name,
 )
 
-from spotify_dl.youtube import download_songs, default_filename, playlist_num_filename, dump_json
+from spotify_dl.youtube import (
+    download_songs,
+    default_filename,
+    playlist_num_filename,
+    dump_json,
+)
 
 
 def spotify_dl():
     """Main entry point of the script."""
     parser = argparse.ArgumentParser(prog="spotify_dl")
     parser.add_argument(
         "-l",
@@ -50,15 +55,15 @@
         default=True,
     )
     parser.add_argument(
         "-j",
         "--dump-json",
         action="store_true",
         help="Dump info-json using youtube-dl",
-        default=False
+        default=False,
     )
     parser.add_argument(
         "-f",
         "--format_str",
         type=str,
         action="store",
         help="Specify youtube-dl format string.",
@@ -91,16 +96,16 @@
         help="Whether we should avoid overwriting the target audio file if it already exists",
         default=False,
     )
     parser.add_argument(
         "-r",
         "--remove-trailing-tracks",
         default="no",
-        action="store_true",
-        help="Whether we should delete tracks that were previously downloaded but are not longer in the playlist"
+        action="store",
+        help="Whether we should delete tracks that were previously downloaded but are not longer in the playlist",
     )
     parser.add_argument(
         "-V",
         "--verbose",
         action="store_true",
         help="Show more information on what" "s happening.",
     )
@@ -139,15 +144,15 @@
     log.debug("Setting debug mode on spotify_dl")
 
     if args.multi_core > (num_cores - 1):
         log.info(
             "Requested cores %d exceeds available %d, using %d cores.",
             args.multi_core,
             num_cores,
-            num_cores - 1
+            num_cores - 1,
         )
         args.multi_core = num_cores - 1
     if args.version:
         console.print(f"spotify_dl [bold green]v{VERSION}[/bold green]")
         sys.exit(0)
 
     if os.path.isfile(os.path.expanduser("~/.spotify_dl_settings")):
@@ -173,36 +178,30 @@
 
     sp = spotipy.Spotify(
         auth_manager=SpotifyClientCredentials(
             client_id=client_id, client_secret=client_secret
         )
     )
     log.debug("Arguments: %s ", args)
-    log.info(
-        "Sponsorblock enabled?: %s",
-        args.use_sponsorblock
-    )
+    log.info("Sponsorblock enabled?: %s", args.use_sponsorblock)
     valid_urls = validate_spotify_urls(args.url)
     if not valid_urls:
         sys.exit(1)
 
     url_data = {"urls": []}
-
+    start_time = time.time()
     for url in valid_urls:
         url_dict = {}
         item_type, item_id = parse_spotify_url(url)
         directory_name = get_item_name(sp, item_type, item_id)
         url_dict["save_path"] = Path(
             PurePath.joinpath(Path(args.output), Path(directory_name))
         )
         url_dict["save_path"].mkdir(parents=True, exist_ok=True)
-        log.info(
-            "Saving songs to %s directory",
-            directory_name
-        )
+        log.info("Saving songs to %s directory", directory_name)
         url_dict["songs"] = fetch_tracks(sp, item_type, url)
         url_data["urls"].append(url_dict.copy())
     if args.dump_json is True:
         dump_json(url_dict["songs"])
     elif args.download is True:
         file_name_f = default_filename
         if args.keep_playlist_order:
@@ -211,22 +210,18 @@
         download_songs(
             songs=url_data,
             output_dir=args.output,
             format_str=args.format_str,
             skip_mp3=args.skip_mp3,
             keep_playlist_order=args.keep_playlist_order,
             no_overwrites=args.no_overwrites,
-            remove_trailing_tracks=args.remove_trailing_tracks,
+            remove_trailing_tracks=(args.remove_trailing_tracks[0].lower()),
             use_sponsorblock=args.use_sponsorblock,
             file_name_f=file_name_f,
             multi_core=args.multi_core,
             proxy=args.proxy,
         )
+    log.info("Download completed in %.2f seconds.", time.time() - start_time)
 
 
 if __name__ == "__main__":
-    start_time = time.time()
     spotify_dl()
-    log.info(
-        "Download completed in %f seconds.", 
-        time.time() - start_time
-    )
```

### Comparing `spotify_dl-8.8.0/spotify_dl/youtube.py` & `spotify_dl-8.8.1/spotify_dl/youtube.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,29 @@
 
 def dump_json(songs):
     """
     Outputs the JSON response of ydl.extract_info to stdout
     :param songs: the songs for which the JSON should be output
     """
     for song in songs:
-        query = f"{song.get('artist')} - {song.get('name')} Lyrics".replace(":", "").replace("\"", "")
+        query = f"{song.get('artist')} - {song.get('name')} Lyrics".replace(
+            ":", ""
+        ).replace('"', "")
 
-        ydl_opts = {
-            'quiet': True
-        }
+        ydl_opts = {"quiet": True}
 
         with yt_dlp.YoutubeDL(ydl_opts) as ydl:
             try:
-                ytJson = ydl.extract_info('ytsearch:' + query, False)
-                print(json.dumps(ytJson.get('entries')))
+                ytJson = ydl.extract_info("ytsearch:" + query, False)
+                print(json.dumps(ytJson.get("entries")))
             except Exception as e:  # skipcq: PYL-W0703
                 log.debug(e)
-                print(f"Failed to download {song.get('name')}, make sure yt_dlp is up to date")
+                print(
+                    f"Failed to download {song.get('name')}, make sure yt_dlp is up to date"
+                )
                 continue
 
 
 def write_tracks(tracks_file, song_dict):
     """
     Writes the information of all tracks in the playlist[s] to a text file in csv kind of format
     This includins the name, artist, and spotify URL. Each is delimited by a comma.
@@ -159,15 +161,14 @@
             print(f"Initiating download for {query}.")
 
             file_name = kwargs["file_name_f"](
                 name=name, artist=artist, track_num=kwargs["track_db"][i].get("num")
             )
 
             if kwargs["use_sponsorblock"][0].lower() == "y":
-
                 sponsorblock_postprocessor = [
                     {
                         "key": "SponsorBlock",
                         "categories": ["skip_non_music_sections"],
                     },
                     {
                         "key": "ModifyChapters",
@@ -184,21 +185,25 @@
                 path_files = set()
                 files[save_path] = path_files
             else:
                 path_files = files[save_path]
 
             path_files.add(f"{file_name}.mp3")
 
-            if kwargs["no_overwrites"] and not kwargs["skip_mp3"] and path.exists(mp3file_path):
-                print(f'File {mp3file_path} already exists, we do not overwrite it ')
+            if (
+                kwargs["no_overwrites"]
+                and not kwargs["skip_mp3"]
+                and path.exists(mp3file_path)
+            ):
+                print(f"File {mp3file_path} already exists, we do not overwrite it ")
                 continue
 
             outtmpl = f"{file_path}.%(ext)s"
             ydl_opts = {
-                "proxy": kwargs.get('proxy'),
+                "proxy": kwargs.get("proxy"),
                 "default_search": "ytsearch",
                 "format": "bestaudio/best",
                 "outtmpl": outtmpl,
                 "postprocessors": sponsorblock_postprocessor,
                 "noplaylist": True,
                 "no_color": False,
                 "postprocessor_args": [
@@ -221,15 +226,15 @@
                 try:
                     ydl.download([query])
                 except Exception as e:  # skipcq: PYL-W0703
                     log.debug(e)
                     print(f"Failed to download {name}, make sure yt_dlp is up to date")
             if not kwargs["skip_mp3"]:
                 set_tags(temp, mp3file_path, kwargs)
-        if kwargs["remove_trailing_tracks"]:
+        if kwargs["remove_trailing_tracks"] == "y":
             for save_path in files:
                 for f in os.listdir(save_path):
                     if f not in files[save_path]:
                         print(f"File {f} is not in the playlist anymore, we delete it")
                         os.remove(path.join(save_path, f))
```

### Comparing `spotify_dl-8.8.0/spotify_dl.egg-info/PKG-INFO` & `spotify_dl-8.8.1/spotify_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-dl
-Version: 8.8.0
+Version: 8.8.1
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

