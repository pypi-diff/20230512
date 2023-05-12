# Comparing `tmp/finny_scraper-0.7.1.tar.gz` & `tmp/finny_scraper-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finny_scraper-0.7.1.tar", last modified: Fri Mar 31 08:29:08 2023, max compression
+gzip compressed data, was "finny_scraper-0.9.tar", last modified: Fri May 12 18:16:08 2023, max compression
```

## Comparing `finny_scraper-0.7.1.tar` & `finny_scraper-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 samtanner   (501) staff       (20)        0 2023-03-31 08:29:08.616655 finny_scraper-0.7.1/
--rw-r--r--   0 samtanner   (501) staff       (20)     1320 2023-03-31 08:29:08.616248 finny_scraper-0.7.1/PKG-INFO
--rw-r--r--   0 samtanner   (501) staff       (20)      788 2023-03-22 22:18:41.000000 finny_scraper-0.7.1/README.md
-drwxr-xr-x   0 samtanner   (501) staff       (20)        0 2023-03-31 08:29:08.614062 finny_scraper-0.7.1/finny_scraper/
--rw-r--r--   0 samtanner   (501) staff       (20)       40 2023-03-23 00:35:32.000000 finny_scraper-0.7.1/finny_scraper/__init__.py
--rw-r--r--   0 samtanner   (501) staff       (20)     8348 2023-03-31 08:28:03.000000 finny_scraper-0.7.1/finny_scraper/finny_scraper.py
-drwxr-xr-x   0 samtanner   (501) staff       (20)        0 2023-03-31 08:29:08.615873 finny_scraper-0.7.1/finny_scraper.egg-info/
--rw-r--r--   0 samtanner   (501) staff       (20)     1320 2023-03-31 08:29:08.000000 finny_scraper-0.7.1/finny_scraper.egg-info/PKG-INFO
--rw-r--r--   0 samtanner   (501) staff       (20)      259 2023-03-31 08:29:08.000000 finny_scraper-0.7.1/finny_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 samtanner   (501) staff       (20)        1 2023-03-31 08:29:08.000000 finny_scraper-0.7.1/finny_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 samtanner   (501) staff       (20)       24 2023-03-31 08:29:08.000000 finny_scraper-0.7.1/finny_scraper.egg-info/requires.txt
--rw-r--r--   0 samtanner   (501) staff       (20)       14 2023-03-31 08:29:08.000000 finny_scraper-0.7.1/finny_scraper.egg-info/top_level.txt
--rw-r--r--   0 samtanner   (501) staff       (20)       38 2023-03-31 08:29:08.616745 finny_scraper-0.7.1/setup.cfg
--rw-r--r--   0 samtanner   (501) staff       (20)      741 2023-03-31 08:28:38.000000 finny_scraper-0.7.1/setup.py
+drwxr-xr-x   0 samtanner   (501) staff       (20)        0 2023-05-12 18:16:08.835453 finny_scraper-0.9/
+-rw-r--r--   0 samtanner   (501) staff       (20)     1158 2023-05-12 18:16:08.835332 finny_scraper-0.9/PKG-INFO
+-rwxrwxrwx   0 samtanner   (501) staff       (20)      788 2023-03-22 22:18:40.000000 finny_scraper-0.9/README.md
+drwxr-xr-x   0 samtanner   (501) staff       (20)        0 2023-05-12 18:16:08.834351 finny_scraper-0.9/finny_scraper/
+-rwxrwxrwx   0 samtanner   (501) staff       (20)       40 2023-03-23 00:35:32.000000 finny_scraper-0.9/finny_scraper/__init__.py
+-rwxrwxrwx   0 samtanner   (501) staff       (20)    12141 2023-05-12 17:47:25.000000 finny_scraper-0.9/finny_scraper/finny_scraper.py
+drwxr-xr-x   0 samtanner   (501) staff       (20)        0 2023-05-12 18:16:08.835145 finny_scraper-0.9/finny_scraper.egg-info/
+-rwxrwxrwx   0 samtanner   (501) staff       (20)     1158 2023-05-12 18:16:08.000000 finny_scraper-0.9/finny_scraper.egg-info/PKG-INFO
+-rwxrwxrwx   0 samtanner   (501) staff       (20)      259 2023-05-12 18:16:08.000000 finny_scraper-0.9/finny_scraper.egg-info/SOURCES.txt
+-rwxrwxrwx   0 samtanner   (501) staff       (20)        1 2023-05-12 18:16:08.000000 finny_scraper-0.9/finny_scraper.egg-info/dependency_links.txt
+-rwxrwxrwx   0 samtanner   (501) staff       (20)       24 2023-05-12 18:16:08.000000 finny_scraper-0.9/finny_scraper.egg-info/requires.txt
+-rwxrwxrwx   0 samtanner   (501) staff       (20)       14 2023-05-12 18:16:08.000000 finny_scraper-0.9/finny_scraper.egg-info/top_level.txt
+-rw-r--r--   0 samtanner   (501) staff       (20)       38 2023-05-12 18:16:08.835494 finny_scraper-0.9/setup.cfg
+-rwxrwxrwx   0 samtanner   (501) staff       (20)      739 2023-05-12 18:11:29.000000 finny_scraper-0.9/setup.py
```

### Comparing `finny_scraper-0.7.1/README.md` & `finny_scraper-0.9/README.md`

 * *Files identical despite different names*

### Comparing `finny_scraper-0.7.1/finny_scraper/finny_scraper.py` & `finny_scraper-0.9/finny_scraper/finny_scraper.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,23 +8,42 @@
         r = requests.get(self.url, headers={"User-Agent": "Mozilla/5.0"})
         soup = BeautifulSoup(r.text, "html.parser")
         self.results = soup.find(class_="aboveBelowTheRail")
         self.property_object = {}
 
     # Property Image
     def get_property_image(self):
-        images = self.results.find_all(
-            "div", class_="InlinePhotoPreview--Photo")
-        if images:
-            main_image_source = images[0].img['src']
-            self.property_object['image'] =  main_image_source
-            return main_image_source
-        else:
-           self.property_object['image'] = None
-           return None
+        try:
+            images = self.results.find_all(
+                "div", class_="InlinePhotoPreview--Photo")
+            if images:
+                main_image_source = images[0].img['src']
+                self.property_object['image'] = main_image_source
+                return main_image_source
+            else:
+                self.property_object['image'] = None
+                return None
+        except:
+            self.property_object['image'] = None
+            return None
+    # SQFT
+
+    def get_sqft(self):
+        try:
+            sqft_element = self.results.find(
+                'div', class_="sqft-section")
+            if sqft_element:
+                sqft = sqft_element.find(class_="statsValue").text
+                clean_sqft = int(
+                    round(float(sqft.replace(',', '').replace('sqft', '').strip())))
+                self.property_object['sqft'] = clean_sqft
+                return clean_sqft
+        except:
+            self.property_object['sqft'] = None
+            return None
 
     # Listing Price
     def get_listing_price(self):
         house_price_element = self.results.find(
             'div', {'data-rf-test-id': 'abp-price'})
         if house_price_element:
             house_price = house_price_element.find(class_="statsValue").text
@@ -54,18 +73,17 @@
                 return property_type
             else:
                 self.property_object['property_type'] = {
                     'classification': None}
                 return None
         else:
             self.property_object['property_type'] = {
-                    'classification': None, 'units': None}
+                'classification': None, 'units': None}
             return None
 
-
     # Specific Amenities
     def get_number_of_units(self):
         amenities = self.results.find(class_="amenities-container")
         number_of_units_element = amenities.find(
             string=lambda text: text and 'units' in text.lower() and '#' in text.lower() and 'with' not in text.lower())
         if number_of_units_element:
             number_of_units = number_of_units_element.find_next().text
@@ -92,29 +110,33 @@
             else:
                 address = None
             city_state_zip_element = self.results.find(
                 'div', {'data-rf-test-id': 'abp-cityStateZip'})
             if city_state_zip_element:
                 city_state_zip = city_state_zip_element.text
                 city_state_zip_list = city_state_zip.split(',')
-                city = city_state_zip_list[0] if len(city_state_zip_list) > 0 else None
-                state_zip = city_state_zip_list[1] if len(city_state_zip_list) > 1 else None
+                city = city_state_zip_list[0] if len(
+                    city_state_zip_list) > 0 else None
+                state_zip = city_state_zip_list[1] if len(
+                    city_state_zip_list) > 1 else None
                 if state_zip:
                     state_zip_list = state_zip.split()
-                    state = state_zip_list[0] if len(state_zip_list) > 0 else None
-                    zip_code = state_zip_list[1] if len(state_zip_list) > 1 else None
+                    state = state_zip_list[0] if len(
+                        state_zip_list) > 0 else None
+                    zip_code = state_zip_list[1] if len(
+                        state_zip_list) > 1 else None
                 else:
                     state = None
                     zip_code = None
             else:
                 city = None
                 state = None
                 zip_code = None
             self.property_object['address'] = {
-                'county': county,
+                'county': county.upper(),
                 'street_address': address,
                 'city': city,
                 'state': state,
                 'zip_code': zip_code
             }
             return self.property_object['address']
         else:
@@ -125,77 +147,142 @@
                 'state': None,
                 'zip_code': None
             }
             return self.property_object['address']
 
     def get_HOA_dues(self):
         key_details_list = self.results.find(
-        class_="keyDetailsList").find_all("div", class_="keyDetail")
+            class_="keyDetailsList").find_all("div", class_="keyDetail")
         HOA_object = {
             'payment': None,
             'frequency': None
         }
         if key_details_list:
             for detail in key_details_list:
                 header = detail.find('span', class_="header")
                 if header and header.text == "HOA Dues":
                     content = detail.find('span', class_="content").text
                     if content:
-                        clean_content = content.replace('$', '').replace(',', '')
-                        periods = ('month', 'year', 'week', 'day', 'quarter', 'semester')
+                        clean_content = content.replace(
+                            '$', '').replace(',', '')
+                        periods = ('month', 'year', 'week',
+                                   'day', 'quarter', 'semester')
                         clean_content_list = clean_content.split('/')
-                        HOA_object['payment'] = round(float(clean_content_list[0])) if len(clean_content_list) > 0 else None
+                        HOA_object['payment'] = round(float(clean_content_list[0])) if len(
+                            clean_content_list) > 0 else None
                         if len(clean_content_list) > 1:
                             for period in periods:
                                 if period in clean_content_list[1].lower():
                                     HOA_object['frequency'] = period
                                     break
                         else:
                             HOA_object['frequency'] = 'month'
                         self.property_object['hoa'] = HOA_object
                         return content
                     break
         self.property_object['hoa'] = HOA_object
         return HOA_object
-    
+
     def get_payment_info(self):
         payment_info = {
             'property_taxes': None,
             'hoa': None,
             'interest_rate_rf': None,
+            'homeowners_insurance': None
         }
         color_bar_section = self.results.find('div', class_="colorBarLegend")
 
         color_bar_section = self.results.find(
-                'section', class_="MortgageCalculatorSection")
-        monthly_cost_items = color_bar_section.find_all('span', class_="Row--header")
+            'section', class_="MortgageCalculatorSection")
+        monthly_cost_items = color_bar_section.find_all(
+            'span', class_="Row--header")
         for item in monthly_cost_items:
             title = item.text
-            if title == 'Property Taxes':
-                payment_info['property_taxes'] = int(item.next_sibling.text.replace('$','').replace(',',''))
-            if title == 'HOA Dues':
-                payment_info['hoa'] = int(item.next_sibling.text.replace('$','').replace(',',''))
-
-        mortgage_form = self.results.find('div', class_="MortgageCalculatorForm")
-        interest_rate = mortgage_form.find('div', {'class': 'panel-title'}, text='Loan Details').find_next_sibling('div', {'class': 'panel-value'}).text.strip()
+            if title.lower() == 'property taxes':
+                payment_info['property_taxes'] = int(
+                    item.next_sibling.text.replace('$', '').replace(',', ''))
+            if title.lower() == 'hoa dues':
+                payment_info['hoa'] = int(
+                    item.next_sibling.text.replace('$', '').replace(',', ''))
+            if title.lower() == "homeowners' insurance" or title == "homeowner's insurance":
+                payment_info['homeowners_insurance'] = int(
+                    item.next_sibling.text.replace('$', '').replace(',', ''))
+
+        mortgage_form = self.results.find(
+            'div', class_="MortgageCalculatorForm")
+        try:
+            interest_rate = mortgage_form.find('div', {'class': 'panel-title'}, text=lambda text: text and 'loan details' in text.lower(
+            )).find_next_sibling('div', {'class': 'panel-value'}).text.strip()
+        except:
+            interest_rate = None
         if interest_rate:
-            payment_info['interest_rate_rf'] = float(interest_rate.replace('%', '').replace(',',''))
+            payment_info['interest_rate_rf'] = float(
+                interest_rate.replace('%', '').replace(',', ''))
 
         self.property_object['payment_info'] = payment_info
         return payment_info
 
-
     def get_property_info(self):
         self.get_property_image()
         self.get_listing_price()
         self.get_property_type()
         self.get_number_of_units()
         self.get_address_info()
         self.get_HOA_dues()
         self.get_payment_info()
+        self.get_sqft()
         return self.property_object
 
-url = 'https://www.redfin.com/HI/Kailua/711-Wailepo-Pl-96734/unit-107/home/63838271'
-house = PropertyInfo(url)
-house.get_property_info()
-print(house.get_property_info()
-)
+
+class InterestRateInfo:
+    def __init__(self):
+        self.mortgage_list_url = 'https://www.investopedia.com/best-30-year-mortgage-rates-5096821'
+        self.piggy_back_url = 'https://www.bankrate.com/home-equity/current-interest-rates/'
+        r_mortgage_list = requests.get(self.mortgage_list_url, headers={
+            "User-Agent": "Mozilla/5.0"})
+        r_piggy_back = requests.get(self.piggy_back_url, headers={
+            "User-Agent": "Mozilla/5.0"})
+        soup_mortgage_list = BeautifulSoup(r_mortgage_list.text, "html.parser")
+        soup_piggy_back = BeautifulSoup(r_piggy_back.text, "html.parser")
+        self.interest_rate_object = {}
+        self.mortgage_list_results = soup_mortgage_list.find(
+            'table', class_="mntl-sc-block-table__table")
+        self.piggy_back_results = soup_piggy_back.find(
+            'table', class_="Table table-content")
+
+    def get_mortgage_rates(self):
+        try:
+            table = self.mortgage_list_results
+            conventional = table.find('td', text='30-Year Fixed').find_next_sibling(
+                'td').text
+            fha = table.find('td', text='FHA 30-Year Fixed').find_next_sibling(
+                'td').text
+            va = table.find('td', text='VA 30-Year Fixed').find_next_sibling(
+                'td').text
+            jumbo = table.find('td', text='Jumbo 30-Year Fixed').find_next_sibling(
+                'td').text
+            self.interest_rate_object['conventional'] = float(conventional.replace(
+                '%', ''))
+            self.interest_rate_object['fha'] = float(fha.replace('%', ''))
+            self.interest_rate_object['va'] = float(va.replace('%', ''))
+            self.interest_rate_object['jumbo'] = float(jumbo .replace('%', ''))
+        except:
+            self.interest_rate_object['conventional'] = None
+            self.interest_rate_object['fha'] = None
+            self.interest_rate_object['va'] = None
+            self.interest_rate_object['jumbo'] = None
+
+    def get_piggy_back_rates(self):
+        try:
+            table = self.piggy_back_results
+            heloc = table.find(
+                'td', string=lambda text: text and 'heloc' in text.lower())
+            rate = heloc.find_next_sibling('td').text
+            self.interest_rate_object['piggy_back'] = float(rate.replace(
+                '%', '').replace('\n', ''))
+        except:
+            self.interest_rate_object['piggy_back'] = None
+
+    def get_interest_rate_info(self):
+        self.get_mortgage_rates()
+        self.get_piggy_back_rates()
+        return self.interest_rate_object
```

### Comparing `finny_scraper-0.7.1/finny_scraper.egg-info/PKG-INFO` & `finny_scraper-0.9/finny_scraper.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: finny-scraper
-Version: 0.7.1
+Version: 0.9
 Summary: A package for scraping property information from Finny website
 Home-page: https://github.com/samueltanner/rfin_scraper
-License: UNKNOWN
-Description: # rfin_scraper
-        a scraper for basic property info on the MLS
-        
-        This can be installed into a project using pip install finny_scrapper in a Python project
-        
-        A new instance of a property class must be created and a redfin url must be passed as the only argument.
-        
-        The accessible methods are:
-        
-        get_property_image() - returns the first image in the property listing as a string
-        get_listing_price() - returns an integer of the current listed property price
-        get_property_type() - returns a string that will be something like "Single Family" or "Multifamily (2-4)" or "C, (2-4)," etc.
-        get_number_of_units() - returns an integer of units on the property. Single Family = 1, Duplex = 2. There are some bugs with condos
-        get_property_info() - return an object with all of the above info in a dictionary
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+
+# rfin_scraper
+a scraper for basic property info on the MLS
+
+This can be installed into a project using pip install finny_scrapper in a Python project
+
+A new instance of a property class must be created and a redfin url must be passed as the only argument.
+
+The accessible methods are:
+
+get_property_image() - returns the first image in the property listing as a string
+get_listing_price() - returns an integer of the current listed property price
+get_property_type() - returns a string that will be something like "Single Family" or "Multifamily (2-4)" or "C, (2-4)," etc.
+get_number_of_units() - returns an integer of units on the property. Single Family = 1, Duplex = 2. There are some bugs with condos
+get_property_info() - return an object with all of the above info in a dictionary
```

### Comparing `finny_scraper-0.7.1/setup.py` & `finny_scraper-0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='finny_scraper',
-    version='0.7.1',
+    version='0.9',
     description='A package for scraping property information from Finny website',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/samueltanner/rfin_scraper',
     packages=['finny_scraper'],
     install_requires=[
         'beautifulsoup4',
```

