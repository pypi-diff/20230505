# Comparing `tmp/IMDbTraktSyncer-1.0.5.tar.gz` & `tmp/IMDbTraktSyncer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.0.5.tar", last modified: Sun Apr 30 07:06:53 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.0.6.tar", last modified: Fri May  5 01:46:54 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.0.5.tar` & `IMDbTraktSyncer-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 07:06:53.519410 IMDbTraktSyncer-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-04-30 07:06:53.455427 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0     6974 2023-04-30 06:58:10.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     2280 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3825 2023-04-29 23:02:25.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1835 2023-04-29 22:57:30.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1782 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:06:53.516414 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     5850 2023-04-30 07:06:53.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-04-30 07:06:53.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 07:06:53.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-30 07:06:53.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-04-30 07:06:53.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-30 07:06:53.000000 IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     5850 2023-04-30 07:06:53.518913 IMDbTraktSyncer-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5242 2023-04-29 21:54:18.000000 IMDbTraktSyncer-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 07:06:53.519910 IMDbTraktSyncer-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-04-30 07:06:15.000000 IMDbTraktSyncer-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:46:54.870618 IMDbTraktSyncer-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-05 01:46:54.835159 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0     6906 2023-05-05 01:45:00.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 01:37:55.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      642 2023-04-30 07:12:26.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3596 2023-05-05 01:45:38.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1401 2023-05-05 01:41:48.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2094 2023-05-05 01:34:29.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:46:54.868115 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     5945 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 01:46:54.000000 IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5945 2023-05-05 01:46:54.870114 IMDbTraktSyncer-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5335 2023-05-05 01:46:16.000000 IMDbTraktSyncer-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 01:46:54.871111 IMDbTraktSyncer-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-05-05 01:40:55.000000 IMDbTraktSyncer-1.0.6/setup.py
```

### Comparing `IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,28 +21,22 @@
     import traktRatings
     import imdbRatings
 from chromedriver_py import binary_path
 
 
 def main():
 
-    here = os.path.abspath(os.path.dirname(__file__))
-    file_path = os.path.join(here, 'credentials.txt')
-    with open(file_path, "r") as f:
-        lines = f.readlines()
-    values = {}
-    for line in lines:
-        key, value = line.strip().split("=")
-        values[key] = value
-    trakt_client_id = values["trakt_client_id"]
-    trakt_client_secret = values["trakt_client_secret"]
-    trakt_access_token = values["trakt_access_token"]
-    imdb_username = values["imdb_username"]
-    imdb_password = values["imdb_password"]
+    #Get credentials
+    trakt_client_id = verifyCredentials.trakt_client_id
+    trakt_client_secret = verifyCredentials.trakt_client_secret
+    trakt_access_token = verifyCredentials.trakt_access_token
+    imdb_username = verifyCredentials.imdb_username
+    imdb_password = verifyCredentials.imdb_password
 
+    #Start web driver
     options = Options()
     options.add_argument("--headless=new")
     options.add_argument('--disable-notifications')
     options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
 
     service = Service(executable_path=binary_path)
     driver = webdriver.Chrome(service=service, options=options)
@@ -76,16 +70,18 @@
     if "Sign In" in element.text:
         print("Not signed in")
     else:
         print("Signed in")
         
     print('Setting IMDB Ratings')
         
+    #Get trakt and imdb ratings and filter out trakt ratings wish missing imbd id
     trakt_ratings = [rating for rating in traktRatings.trakt_ratings if rating['ID'] is not None]
     imdb_ratings = [rating for rating in imdbRatings.imdb_ratings if rating['ID'] is not None]
+    #Filter out ratings already set
     imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [imdb_rating['ID'] for imdb_rating in imdb_ratings]]
     trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
 
     # loop through each movie and TV show rating and submit rating on IMDb website
     for i, item in enumerate(imdb_ratings_to_set, 1):
         print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]} ({item["Year"]}): {item["Rating"]}/10 on IMDb')
         driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
@@ -157,14 +153,14 @@
         while response.status_code == 429:
             print("Rate limit exceeded. Waiting for 1 second...")
             time.sleep(1)
             response = requests.post(rate_url, headers=headers, json=data)
         if response.status_code != 201:
             print(f"Error rating {item}: {response.content}")
 
-
+    #Close web driver
     print("Closing webdriver...")
     driver.quit()
     service.stop()
 
 if __name__ == '__main__':
     main()
```

### Comparing `IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/authTrakt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,49 @@
 import requests
 import os
 
-here = os.path.abspath(os.path.dirname(__file__))
-file_path = os.path.join(here, 'credentials.txt')
-
-with open(file_path, "r") as f:
-    lines = f.readlines()
-values = {}
-for line in lines:
-    key, value = line.strip().split("=")
-    values[key] = value
-CLIENT_ID = values["trakt_client_id"]
-CLIENT_SECRET = values["trakt_client_secret"]
-REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
-
-# Set up the authorization endpoint URL
-auth_url = 'https://trakt.tv/oauth/authorize'
-
-# Construct the authorization URL with the necessary parameters
-params = {
-    'response_type': 'code',
-    'client_id': CLIENT_ID,
-    'redirect_uri': REDIRECT_URI,
-    'state': 'mystate', # Optional - used for CSRF protection
-}
-auth_url += '?' + '&'.join([f'{key}={value}' for key, value in params.items()])
-
-# Print out the authorization URL and instruct the user to visit it
-print(f'\nPlease visit the following URL to authorize this application: \n{auth_url}\n')
-
-# After the user grants authorization, they will be redirected back to the redirect URI with a temporary authorization code.
-# Extract the authorization code from the URL and use it to request an access token from the Trakt API.
-authorization_code = input('Please enter the authorization code from the URL: ')
-
-# Set up the access token request
-headers = {
-    'Content-Type': 'application/json'
-}
-data = {
-    'code': authorization_code,
-    'client_id': CLIENT_ID,
-    'client_secret': CLIENT_SECRET,
-    'redirect_uri': REDIRECT_URI,
-    'grant_type': 'authorization_code'
-}
-
-# Make the request to get the access token
-response = requests.post('https://api.trakt.tv/oauth/token', headers=headers, json=data)
-
-# Parse the JSON response from the API
-json_data = response.json()
-
-# Extract the access token from the response
-ACCESS_TOKEN = json_data['access_token']
-
-# Save the access token value to the credentials file
-with open(file_path, "w") as f:
-    for key, value in values.items():
-        if key == "trakt_access_token":
-            f.write(f"{key}={ACCESS_TOKEN}\n")
-        else:
-            f.write(f"{key}={value}\n")
-
-# Print out a message indicating that the token has been saved
-print(f'Trakt access token saved to credentials.txt')
+def authenticate(client_id, client_secret):
+    CLIENT_ID = client_id
+    CLIENT_SECRET = client_secret
+    REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
+
+    # Set up the authorization endpoint URL
+    auth_url = 'https://trakt.tv/oauth/authorize'
+
+    # Construct the authorization URL with the necessary parameters
+    params = {
+        'response_type': 'code',
+        'client_id': CLIENT_ID,
+        'redirect_uri': REDIRECT_URI,
+        'state': 'mystate', # Optional - used for CSRF protection
+    }
+    auth_url += '?' + '&'.join([f'{key}={value}' for key, value in params.items()])
+
+    # Print out the authorization URL and instruct the user to visit it
+    print(f'\nPlease visit the following URL to authorize this application: \n{auth_url}\n')
+
+    # After the user grants authorization, they will be redirected back to the redirect URI with a temporary authorization code.
+    # Extract the authorization code from the URL and use it to request an access token from the Trakt API.
+    authorization_code = input('Please enter the authorization code from the URL: ')
+
+    # Set up the access token request
+    headers = {
+        'Content-Type': 'application/json'
+    }
+    data = {
+        'code': authorization_code,
+        'client_id': CLIENT_ID,
+        'client_secret': CLIENT_SECRET,
+        'redirect_uri': REDIRECT_URI,
+        'grant_type': 'authorization_code'
+    }
+
+    # Make the request to get the access token
+    response = requests.post('https://api.trakt.tv/oauth/token', headers=headers, json=data)
+
+    # Parse the JSON response from the API
+    json_data = response.json()
+
+    # Extract the access token from the response
+    ACCESS_TOKEN = json_data['access_token']
+    
+    return ACCESS_TOKEN
```

### Comparing `IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/imdbRatings.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from chromedriver_py import binary_path
+try:
+    from IMDbTraktSyncer import verifyCredentials
+except:
+    import verifyCredentials
 
+#Get IMDb Ratings
 print('Getting IMDB Ratings')
 
-here = os.path.abspath(os.path.dirname(__file__))
-file_path = os.path.join(here, 'credentials.txt')
-with open(file_path, "r") as f:
-    lines = f.readlines()
-values = {}
-for line in lines:
-    key, value = line.strip().split("=")
-    values[key] = value
-imdb_username = values["imdb_username"]
-imdb_password = values["imdb_password"]
+imdb_username = verifyCredentials.imdb_username
+imdb_password = verifyCredentials.imdb_password
 
 directory = os.path.dirname(os.path.realpath(__file__))
+
+#Start web driver
 options = Options()
 options.add_argument("--headless=new")
 options.add_argument('--disable-notifications')
 options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
 options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False})
 
 
@@ -41,16 +40,16 @@
 sign_in_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '.auth-provider-text')))
 if sign_in_link.text == 'Sign in with IMDb':
     sign_in_link.click()
 
 email_input = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, "input[type='email']")))[0]
 password_input = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, "input[type='password']")))[0]
 
-email_input.send_keys(values["imdb_username"])
-password_input.send_keys(values["imdb_password"])
+email_input.send_keys(imdb_username)
+password_input.send_keys(imdb_password)
 
 submit_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input[type='submit']")))
 submit_button.click()
 time.sleep(3)
 
 driver.get('https://www.imdb.com/list/ratings')
 
@@ -64,22 +63,23 @@
 
 dropdown = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".circle")))
 dropdown.click()
 
 csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".pop-up-menu-list-items a.pop-up-menu-list-item-link")))
 csv_link.click()
 
-#Wait for csv download to complete
+#Wait for csv download to complete and close web driver
 time.sleep(10)
 driver.quit()
 service.stop()
 
 imdb_ratings = []
 
 # Read the ratings from the CSV file
+here = os.path.abspath(os.path.dirname(__file__))
 ratings_path = os.path.join(here, 'ratings.csv')
 try:
     with open(ratings_path, 'r') as file:
         reader = csv.reader(file)
         header = next(reader)  # skip the header row
         for row in reader:
             title = row[3]
@@ -95,14 +95,10 @@
     print('Ratings file not found')
     
 # Delete csv files
 for file in os.listdir(directory):
     if file.endswith('.csv'):
         os.remove(os.path.join(directory, file))
 
-# Print the results
-#for rating in imdb_ratings:
-#    print(f'Title: {rating["Title"]}, Year: {rating["Year"]}, Rating: {rating["Rating"]}, IMDB ID: {rating["ID"]}')
-
 print('Getting IMDB Ratings Complete')
```

### Comparing `IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/traktRatings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import os
 import json
 import subprocess
-import requests 
+import requests
+try:
+    from IMDbTraktSyncer import verifyCredentials
+except:
+    import verifyCredentials
 
+#Get Trakt Ratings
 print('Getting Trakt Ratings')
 
-here = os.path.abspath(os.path.dirname(__file__))
-file_path = os.path.join(here, 'credentials.txt')
-with open(file_path, "r") as f:
-    lines = f.readlines()
-values = {}
-for line in lines:
-    key, value = line.strip().split("=")
-    values[key] = value
-CLIENT_ID = values["trakt_client_id"]
-ACCESS_TOKEN = values["trakt_access_token"]
+CLIENT_ID = verifyCredentials.trakt_client_id
+ACCESS_TOKEN = verifyCredentials.trakt_access_token
 
 headers = {
     'Content-Type': 'application/json',
     'trakt-api-version': '2',
     'trakt-api-key': CLIENT_ID,
     'Authorization': f'Bearer {ACCESS_TOKEN}'
 }
@@ -40,16 +37,8 @@
     elif item['type'] == 'show':
         show = item['show']
         show_id = show['ids']['imdb']
         show_ratings.append({'Title': show['title'], 'Year': show['year'], 'Rating': item['rating'], 'ID': show_id, 'Type': 'show'})
 
 trakt_ratings = movie_ratings + show_ratings
 
-#print('Movie ratings:')
-#for item in movie_ratings:
-#    print(f'{item["Title"]} ({item["Year"]}): {item["Rating"]}/10 (IMDb ID: {item["ID"]})')
-#
-#print('\nShow ratings:')
-#for item in show_ratings:
-#    print(f'{item["Title"]} ({item["Year"]}): {item["Rating"]}/10 (IMDb ID: {item["ID"]})')
-
 print('Getting Trakt Ratings Complete')
```

### Comparing `IMDbTraktSyncer-1.0.5/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer/verifyCredentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 import os
+try:
+    from IMDbTraktSyncer import authTrakt
+except:
+    import authTrakt
 
 # Define the file path
 here = os.path.abspath(os.path.dirname(__file__))
 file_path = os.path.join(here, 'credentials.txt')
 
 # Check if the file exists
 if not os.path.isfile(file_path):
@@ -28,22 +32,26 @@
 for key in values.keys():
     if values[key] == "empty" and key != "trakt_access_token":
         values[key] = input(f"Please enter a value for {key}: ")
         with open(file_path, "w") as f:
             for key, value in values.items():
                 f.write(f"{key}={value}\n")
 
-# Get the trakt_access_token value if it exists, or run the authTrakt.py script to get it
+# Get the trakt_access_token value if it exists, or run the authTrakt.py function to get it
 trakt_access_token = None
 if "trakt_access_token" in values and values["trakt_access_token"] != "empty":
     trakt_access_token = values["trakt_access_token"]
 else:
-    here = os.path.abspath(os.path.dirname(__file__))
-    authTraktPath = os.path.join(here, 'authTrakt.py')
-    os.system(f"python {authTraktPath}")
-    with open(file_path, "r") as f:
-        lines = f.readlines()
-    for line in lines:
-        key, value = line.strip().split("=")
-        if key == "trakt_access_token":
-            trakt_access_token = value
-            break
+    client_id = values["trakt_client_id"]
+    client_secret = values["trakt_client_secret"]
+    trakt_access_token = authTrakt.authenticate(client_id, client_secret)
+    values["trakt_access_token"] = trakt_access_token
+    with open(file_path, "w") as f:
+        for key, value in values.items():
+            f.write(f"{key}={value}\n")
+
+# Save the credential values as variables
+trakt_client_id = values["trakt_client_id"]
+trakt_client_secret = values["trakt_client_secret"]
+trakt_access_token = values["trakt_access_token"]
+imdb_username = values["imdb_username"]
+imdb_password = values["imdb_password"]
```

### Comparing `IMDbTraktSyncer-1.0.5/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.0.6/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.5
+Version: 1.0.6
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python is supported.
+This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Run the script by calling `IMDbTraktSyncer` in command line. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-5. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+4. Run the script by calling `IMDbTraktSyncer` in command line. 
+5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Run:
 `IMDbTraktSyncer` in command line.
 
 ## Update:
 `python -m pip install IMDbTraktSyncer --upgrade` in command line.
 
 ## Uninstall:
 `python -m pip uninstall IMDbTraktSyncer` in command line.
 
-## Alternative manual install method:
+## Alternative manual no install method:
 1. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and move it to the file directory of your choice.
-2. Open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+2. Run `IMDbTraktSyncer.py` OR open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. 
+3. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+4. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Troubleshooting, known issues, workarounds & future outlook:
 * IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
 * If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
 * Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
```

### Comparing `IMDbTraktSyncer-1.0.5/LICENSE` & `IMDbTraktSyncer-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.5/PKG-INFO` & `IMDbTraktSyncer-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.5
+Version: 1.0.6
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python is supported.
+This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Run the script by calling `IMDbTraktSyncer` in command line. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-5. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+4. Run the script by calling `IMDbTraktSyncer` in command line. 
+5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Run:
 `IMDbTraktSyncer` in command line.
 
 ## Update:
 `python -m pip install IMDbTraktSyncer --upgrade` in command line.
 
 ## Uninstall:
 `python -m pip uninstall IMDbTraktSyncer` in command line.
 
-## Alternative manual install method:
+## Alternative manual no install method:
 1. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and move it to the file directory of your choice.
-2. Open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+2. Run `IMDbTraktSyncer.py` OR open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. 
+3. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+4. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Troubleshooting, known issues, workarounds & future outlook:
 * IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
 * If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
 * Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
```

### Comparing `IMDbTraktSyncer-1.0.5/README.md` & `IMDbTraktSyncer-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python is supported.
+This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Run the script by calling `IMDbTraktSyncer` in command line. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-5. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+4. Run the script by calling `IMDbTraktSyncer` in command line. 
+5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Run:
 `IMDbTraktSyncer` in command line.
 
 ## Update:
 `python -m pip install IMDbTraktSyncer --upgrade` in command line.
 
 ## Uninstall:
 `python -m pip uninstall IMDbTraktSyncer` in command line.
 
-## Alternative manual install method:
+## Alternative manual no install method:
 1. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and move it to the file directory of your choice.
-2. Open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+2. Run `IMDbTraktSyncer.py` OR open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. 
+3. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+4. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Troubleshooting, known issues, workarounds & future outlook:
 * IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
 * If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
 * Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
```

### Comparing `IMDbTraktSyncer-1.0.5/setup.py` & `IMDbTraktSyncer-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = 'This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

