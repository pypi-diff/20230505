# Comparing `tmp/shazamio-0.3.1.1.tar.gz` & `tmp/shazamio-0.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shazamio-0.3.1.1.tar", max compression
+gzip compressed data, was "shazamio-0.4.0.0.tar", max compression
```

## Comparing `shazamio-0.3.1.1.tar` & `shazamio-0.4.0.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1063 2022-12-29 14:11:19.891984 shazamio-0.3.1.1/LICENSE.txt
--rw-r--r--   0        0        0    10231 2022-12-29 14:11:19.891984 shazamio-0.3.1.1/README.md
--rw-r--r--   0        0        0     1036 2022-12-29 14:11:39.375785 shazamio-0.3.1.1/pyproject.toml
--rw-r--r--   0        0        0      172 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/__init__.py
--rw-r--r--   0        0        0    11516 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/algorithm.py
--rw-r--r--   0        0        0    13602 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/api.py
--rw-r--r--   0        0        0      667 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/client.py
--rw-r--r--   0        0        0     2509 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/converter.py
--rw-r--r--   0        0        0      832 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/enums.py
--rw-r--r--   0        0        0      168 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/exceptions.py
--rw-r--r--   0        0        0     3459 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/factory.py
--rw-r--r--   0        0        0     1526 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/factory_misc.py
--rw-r--r--   0        0        0     2659 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/misc.py
--rw-r--r--   0        0        0        0 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/__init__.py
--rw-r--r--   0        0        0        0 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/artist/__init__.py
--rw-r--r--   0        0        0        0 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/artist/views/__init__.py
--rw-r--r--   0        0        0     1863 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/artist/views/full_albums.py
--rw-r--r--   0        0        0     1487 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/artist/views/last_release.py
--rw-r--r--   0        0        0     1337 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/artist/views/simular_artists.py
--rw-r--r--   0        0        0     1406 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/artist/views/top_music.py
--rw-r--r--   0        0        0     2627 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/artists.py
--rw-r--r--   0        0        0      345 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/attributes.py
--rw-r--r--   0        0        0      455 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/base.py
--rw-r--r--   0        0        0      464 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/enums.py
--rw-r--r--   0        0        0      138 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/errors.py
--rw-r--r--   0        0        0     4114 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/models.py
--rw-r--r--   0        0        0      526 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/schemas/photos.py
--rw-r--r--   0        0        0      956 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/serializers.py
--rw-r--r--   0        0        0     9880 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/signature.py
--rw-r--r--   0        0        0      164 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/typehints.py
--rw-r--r--   0        0        0     7017 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/user_agent.py
--rw-r--r--   0        0        0     1863 2022-12-29 14:11:19.895984 shazamio-0.3.1.1/shazamio/utils.py
--rw-r--r--   0        0        0    11697 1970-01-01 00:00:00.000000 shazamio-0.3.1.1/setup.py
--rw-r--r--   0        0        0    11364 1970-01-01 00:00:00.000000 shazamio-0.3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-05 06:25:35.115534 shazamio-0.4.0.0/LICENSE.txt
+-rw-r--r--   0        0        0    10440 2023-05-05 06:25:35.115534 shazamio-0.4.0.0/README.md
+-rw-r--r--   0        0        0     1036 2023-05-05 06:25:51.027648 shazamio-0.4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/__init__.py
+-rw-r--r--   0        0        0    11516 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/algorithm.py
+-rw-r--r--   0        0        0    14285 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/api.py
+-rw-r--r--   0        0        0      667 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/client.py
+-rw-r--r--   0        0        0     2509 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/converter.py
+-rw-r--r--   0        0        0      832 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/enums.py
+-rw-r--r--   0        0        0      168 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/exceptions.py
+-rw-r--r--   0        0        0     3458 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/factory.py
+-rw-r--r--   0        0        0     1526 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/factory_misc.py
+-rw-r--r--   0        0        0     2805 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/misc.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/__init__.py
+-rw-r--r--   0        0        0     1863 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/full_albums.py
+-rw-r--r--   0        0        0     1487 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/last_release.py
+-rw-r--r--   0        0        0     1337 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/simular_artists.py
+-rw-r--r--   0        0        0     1406 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/top_music.py
+-rw-r--r--   0        0        0     1817 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artist/views/top_song.py
+-rw-r--r--   0        0        0     2752 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/artists.py
+-rw-r--r--   0        0        0      345 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/attributes.py
+-rw-r--r--   0        0        0      455 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/base.py
+-rw-r--r--   0        0        0      464 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/enums.py
+-rw-r--r--   0        0        0      138 2023-05-05 06:25:35.127534 shazamio-0.4.0.0/shazamio/schemas/errors.py
+-rw-r--r--   0        0        0     4122 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/schemas/models.py
+-rw-r--r--   0        0        0      526 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/schemas/photos.py
+-rw-r--r--   0        0        0       71 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/schemas/urls.py
+-rw-r--r--   0        0        0      956 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/serializers.py
+-rw-r--r--   0        0        0     9880 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/signature.py
+-rw-r--r--   0        0        0      164 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/typehints.py
+-rw-r--r--   0        0        0     7017 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/user_agent.py
+-rw-r--r--   0        0        0     1863 2023-05-05 06:25:35.131534 shazamio-0.4.0.0/shazamio/utils.py
+-rw-r--r--   0        0        0    11573 1970-01-01 00:00:00.000000 shazamio-0.4.0.0/PKG-INFO
```

### Comparing `shazamio-0.3.1.1/LICENSE.txt` & `shazamio-0.4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/README.md` & `shazamio-0.4.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 import asyncio
 from shazamio import Shazam
 
 
 async def main():
     shazam = Shazam()
     track_id = 546891609
-    related = await shazam.related_tracks(track_id=track_id, limit=5, start_from=2)
+    related = await shazam.related_tracks(track_id=track_id, limit=5, offset=2)
     # ONLY №3, №4 SONG
     print(related)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
   ```
 </details>
@@ -206,27 +206,39 @@
 
 Get the top songs according to Shazam<br>
 <a href="https://www.shazam.com/artist/201896832/kizaru">https://www.shazam.com/artist/201896832/kizaru</a>
 
   ```python3
 import asyncio
 from shazamio import Shazam, Serialize
+from shazamio.schemas.artists import ArtistQuery
+from shazamio.schemas.enums import ArtistView
 
 
 async def main():
     shazam = Shazam()
-    artist_id = 201896832
-    top_three_artist_tracks = await shazam.artist_top_tracks(artist_id=artist_id, limit=3)
-    for track in top_three_artist_tracks['tracks']:
-        serialized_track = Serialize.track(data=track)
-        print(serialized_track)
+    artist_id = 1081606072
 
-loop = asyncio.get_event_loop()
+    about_artist = await shazam.artist_about(
+        artist_id,
+        query=ArtistQuery(
+            views=[
+                ArtistView.TOP_SONGS,
+            ],
+        ),
+    )
+    serialized = Serialize.artist_v2(about_artist)
+    for i in serialized.data[0].views.top_songs.data:
+        print(i.attributes.name)
+
+
+loop = asyncio.get_event_loop_policy().get_event_loop()
 loop.run_until_complete(main())
 
+
   ```
 </details>
 
 <details> 
 <summary>
 <i>🔝🎶🏙️ Top tracks in city</i>
 </summary>
```

#### html2text {}

```diff
@@ -34,34 +34,37 @@
 track/559284007/rampampam shazam = Shazam() track_id = 559284007 count = await
 shazam.listening_counter(track_id=track_id) print(count) loop =
 asyncio.get_event_loop() loop.run_until_complete(main()) ```    ð¶ð¬
 Similar songs  Similar songs based song id
 https://www.shazam.com/track/546891609/2-phu%CC%81t-ho%CC%9Bn-kaiz-remix
 ```python3 import asyncio from shazamio import Shazam async def main(): shazam
 = Shazam() track_id = 546891609 related = await shazam.related_tracks
-(track_id=track_id, limit=5, start_from=2) # ONLY â3, â4 SONG print
-(related) loop = asyncio.get_event_loop() loop.run_until_complete(main()) ```
+(track_id=track_id, limit=5, offset=2) # ONLY â3, â4 SONG print(related)
+loop = asyncio.get_event_loop() loop.run_until_complete(main()) ```
 ðð¨âð¤ Search artists  Search all artists by prefix
 ```python3 import asyncio from shazamio import Shazam, Serialize async def main
 (): shazam = Shazam() artists = await shazam.search_artist(query='Lil',
 limit=5) for artist in artists['artists']['hits']: serialized =
 Serialize.artist(data=artist) print(serialized) loop = asyncio.get_event_loop()
 loop.run_until_complete(main()) ```    ðð¶ Search tracks  Search all
 tracks by prefix
 ```python3 import asyncio from shazamio import Shazam async def main(): shazam
 = Shazam() tracks = await shazam.search_track(query='Lil', limit=5) print
 (tracks) loop = asyncio.get_event_loop() loop.run_until_complete(main()) ```
 ðð¶ð¨âð¤ Top artist tracks  Get the top songs according to Shazam
 https://www.shazam.com/artist/201896832/kizaru ```python3 import asyncio from
-shazamio import Shazam, Serialize async def main(): shazam = Shazam() artist_id
-= 201896832 top_three_artist_tracks = await shazam.artist_top_tracks
-(artist_id=artist_id, limit=3) for track in top_three_artist_tracks['tracks']:
-serialized_track = Serialize.track(data=track) print(serialized_track) loop =
-asyncio.get_event_loop() loop.run_until_complete(main()) ```    ðð¶ðï¸
-Top tracks in city  Retrieving information from an artist profile
+shazamio import Shazam, Serialize from shazamio.schemas.artists import
+ArtistQuery from shazamio.schemas.enums import ArtistView async def main():
+shazam = Shazam() artist_id = 1081606072 about_artist = await
+shazam.artist_about( artist_id, query=ArtistQuery( views=
+[ ArtistView.TOP_SONGS, ], ), ) serialized = Serialize.artist_v2(about_artist)
+for i in serialized.data[0].views.top_songs.data: print(i.attributes.name) loop
+= asyncio.get_event_loop_policy().get_event_loop() loop.run_until_complete(main
+()) ```    ðð¶ðï¸ Top tracks in city  Retrieving information from an
+artist profile
 https://www.shazam.com/charts/top-50/russia/moscow ```python3 import asyncio
 from shazamio import Shazam, Serialize async def main(): shazam = Shazam()
 top_ten_moscow_tracks = await shazam.top_city_tracks(country_code='RU',
 city_name='Moscow', limit=10) print(top_ten_moscow_tracks) # ALL TRACKS DICT
 for track in top_ten_moscow_tracks['tracks']: serialized = Serialize.track
 (data=track) # SERIALIZE FROM DATACLASS FACTORY print(serialized) loop =
 asyncio.get_event_loop() loop.run_until_complete(main()) ```
```

### Comparing `shazamio-0.3.1.1/pyproject.toml` & `shazamio-0.4.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shazamio"
-version = "0.3.1.1"
+version = "0.4.0.0"
 description = "Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp."
 authors = ["dotX12"]
 license = "MIT License"
 keywords = ["python", "shazam", "music", "recognize", "api", "async", "asyncio", "aiohttp", "identification"]
 readme = "README.md"
 homepage = "https://github.com/dotX12/ShazamIO"
 repository = "https://github.com/dotX12/ShazamIO"
```

### Comparing `shazamio-0.3.1.1/shazamio/algorithm.py` & `shazamio-0.4.0.0/shazamio/algorithm.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/api.py` & `shazamio-0.4.0.0/shazamio/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,35 +18,37 @@
 from .utils import get_song
 
 
 class Shazam(Converter, Geo, Request):
     """Is asynchronous framework for reverse engineered Shazam API written in Python 3.7 with
     asyncio and aiohttp."""
 
-    def __init__(self, language: str = "ES"):
+    def __init__(self, language: str = "en-US", endpoint_country: str = "GB"):
         super().__init__(language=language)
         self.language = language
+        self.endpoint_country = endpoint_country
 
-    async def top_world_tracks(self, limit: int = 200, start_from: int = 0) -> Dict[str, Any]:
+    async def top_world_tracks(self, limit: int = 200, offset: int = 0) -> Dict[str, Any]:
         """
         Search top world tracks
 
             :param limit: Determines how many songs the maximum can be in the request.
                 Example: If 5 is specified, the query will return no more than 5 songs.
-            :param start_from: A parameter that determines with which song to display the request.
+            :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :return: dict tracks
         """
         return await self.request(
             "GET",
             ShazamUrl.TOP_TRACKS_WORLD.format(
-                limit,
-                start_from,
                 language=self.language,
+                endpoint_country=self.endpoint_country,
+                limit=limit,
+                offset=offset,
             ),
             headers=self.headers(),
         )
 
     async def artist_about(
         self, artist_id: int, query: Optional[ArtistQuery] = None
     ) -> Dict[str, Any]:
@@ -63,123 +65,109 @@
             pg = ArtistQueryGenerator(source=query)
             params_dict = pg.params()
         else:
             params_dict = {}
 
         return await self.request(
             "GET",
-            ShazamUrl.SEARCH_ARTIST_V2.format(artist_id, language=self.language),
-            params=params_dict,
-            headers=self.headers(),
-        )
-
-    async def artist_top_tracks(
-        self, artist_id: int, limit: int = 200, start_from: int = 0
-    ) -> Dict[str, Any]:
-        """
-        Get the top songs according to Shazam
-
-            :param artist_id: Artist number. Example: (203347991)
-            https://www.shazam.com/artist/203347991/
-            :param limit: Determines how many songs the maximum can be in the request.
-                Example: If 5 is specified, the query will return no more than 5 songs.
-            :param start_from: A parameter that determines with which song to display the request.
-                The default is 0. If you want to skip the first few songs, set this parameter to
-                your own.
-            :return: dict tracks
-        """
-        return await self.request(
-            "GET",
-            ShazamUrl.ARTIST_TOP_TRACKS.format(
-                artist_id, start_from, limit, language=self.language
+            ShazamUrl.SEARCH_ARTIST_V2.format(
+                endpoint_country=self.endpoint_country,
+                artist_id=artist_id,
             ),
+            params=params_dict,
             headers=self.headers(),
         )
 
     async def track_about(self, track_id: int) -> Dict[str, Any]:
         """
         Get track information
 
             :param track_id: Track number. Example: (549952578)
             https://www.shazam.com/track/549952578/
             :return: dict about track
         """
         return await self.request(
             "GET",
             ShazamUrl.ABOUT_TRACK.format(
-                track_id,
                 language=self.language,
+                endpoint_country=self.endpoint_country,
+                track_id=track_id,
             ),
             headers=self.headers(),
         )
 
     async def top_country_tracks(
         self,
         country_code: Union[CountryCode, str],
         limit: int = 200,
-        start_from: int = 0,
+        offset: int = 0,
     ) -> Dict[str, Any]:
         """
         Get the best tracks by country code
         https://www.shazam.com/charts/discovery/netherlands
 
             :param country_code: ISO 3166-3 alpha-2 code. Example: RU,NL,UA
             :param limit: Determines how many songs the maximum can be in the request.
                 Example: If 5 is specified, the query will return no more than 5 songs.
-            :param start_from: A parameter that determines with which song to display the request.
+            :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :return: dict songs
         """
         return await self.request(
             "GET",
             ShazamUrl.TOP_TRACKS_COUNTRY.format(
-                country_code,
-                limit,
-                start_from,
                 language=self.language,
+                endpoint_country=self.endpoint_country,
+                country_code=country_code,
+                limit=limit,
+                offset=offset,
             ),
             headers=self.headers(),
         )
 
     async def top_city_tracks(
         self,
         country_code: Union[CountryCode, str],
         city_name: str,
         limit: int = 200,
-        start_from: int = 0,
+        offset: int = 0,
     ) -> Dict[str, Any]:
         """
         Retrieving information from an artist profile
         https://www.shazam.com/charts/top-50/russia/moscow
 
             :param country_code: ISO 3166-3 alpha-2 code. Example: RU,NL,UA
             :param city_name: City name from https://github.com/dotX12/dotX12/blob/main/city.json
                 Example: Budapest, Moscow
             :param limit: Determines how many songs the maximum can be in the request.
                 Example: If 5 is specified, the query will return no more than 5 songs.
-            :param start_from: A parameter that determines with which song to display the request.
+            :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :return: dict songs
         """
         city_id = await self.city_id_from(country=country_code, city=city_name)
         return await self.request(
             "GET",
             ShazamUrl.TOP_TRACKS_CITY.format(
-                city_id,
-                limit,
-                start_from,
                 language=self.language,
+                endpoint_country=self.endpoint_country,
+                limit=limit,
+                offset=offset,
+                city_id=city_id,
             ),
             headers=self.headers(),
         )
 
     async def top_world_genre_tracks(
-        self, genre: Union[GenreMusic, int], limit: int = 100, start_from: int = 0
+        self,
+        genre: Union[GenreMusic, int],
+        limit: int = 100,
+        offset: int = 0,
     ) -> Dict[str, Any]:
         """
         Get world tracks by certain genre
         https://www.shazam.com/charts/genre/world/rock
 
             :param genre: Genre name or ID:
                 POP = 1, HIP_HOP_RAP = 2, DANCE = 3, ELECTRONIC = 4, RNB_SOUL = 5, ALTERNATIVE =
@@ -187,111 +175,146 @@
                 LATIN = 8, FILM_TV_STAGE = 9, COUNTRY = 10, AFRO_BEATS = 11, WORLDWIDE = 12,
                 REGGAE_DANCE_HALL = 13
                 HOUSE = 14, K_POP = 15, FRENCH_POP = 16, SINGER_SONGWRITER = 17,
                 REGIONAL_MEXICANO = 18
 
             :param limit: Determines how many songs the maximum can be in the request.
                     Example: If 5 is specified, the query will return no more than 5 songs.
-            :param start_from: A parameter that determines with which song to display the request.
+            :param offset: A parameter that determines with which song to display the request.
                     The default is 0. If you want to skip the first few songs, set this parameter
                     to your own.
             :return: dict songs
         """
         return await self.request(
             "GET",
-            ShazamUrl.GENRE_WORLD.format(genre, limit, start_from, language=self.language),
+            ShazamUrl.GENRE_WORLD.format(
+                language=self.language,
+                endpoint_country=self.endpoint_country,
+                limit=limit,
+                offset=offset,
+                genre=genre,
+            ),
             headers=self.headers(),
         )
 
     async def top_country_genre_tracks(
         self,
         country_code: str,
         genre: Union[GenreMusic, int],
         limit: int = 200,
-        start_from: int = 0,
+        offset: int = 0,
     ) -> Dict[str, Any]:
         """
         The best tracks by a genre in the country
         https://www.shazam.com/charts/genre/spain/hip-hop-rap
             :param country_code: ISO 3166-3 alpha-2 code. Example: RU,NL,UA
             :param genre: Genre name or ID:
                 POP = 1, HIP_HOP_RAP = 2, DANCE = 3, ELECTRONIC = 4, RNB_SOUL = 5, ALTERNATIVE =
                 6, ROCK = 7
                 LATIN = 8, FILM_TV_STAGE = 9, COUNTRY = 10, AFRO_BEATS = 11, WORLDWIDE = 12,
                 REGGAE_DANCE_HALL = 13
                 HOUSE = 14, K_POP = 15, FRENCH_POP = 16, SINGER_SONGWRITER = 17,
                 REGIONAL_MEXICANO = 18
             :param limit: Determines how many songs the maximum can be in the request.
                 Example: If 5 is specified, the query will return no more than 5 songs
-            :param start_from: A parameter that determines with which song to display the request.
+            :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :return: dict songs
         """
         return await self.request(
             "GET",
             ShazamUrl.GENRE_COUNTRY.format(
-                country_code, genre, limit, start_from, language=self.language
+                language=self.language,
+                endpoint_country=self.endpoint_country,
+                limit=limit,
+                offset=offset,
+                country=country_code,
+                genre=genre,
             ),
             headers=self.headers(),
         )
 
     async def related_tracks(
-        self, track_id: int, limit: int = 20, start_from: int = 0
+        self,
+        track_id: int,
+        limit: int = 20,
+        offset: int = 0,
     ) -> Dict[str, Any]:
         """
         Similar songs based song id
         https://www.shazam.com/track/546891609/2-phu%CC%81t-ho%CC%9Bn-kaiz-remix
             :param track_id: Track number. Example: (549952578)
             https://www.shazam.com/track/549952578/
             :param limit: Determines how many songs the maximum can be in the request.
                 Example: If 5 is specified, the query will return no more than 5 songs
-            :param start_from: A parameter that determines with which song to display the request.
+            :param offset: A parameter that determines with which song to display the request.
                 The default is 0. If you want to skip the first few songs, set this parameter to
                 your own.
             :return: dict tracks
         """
         return await self.request(
             "GET",
-            ShazamUrl.RELATED_SONGS.format(track_id, start_from, limit, language=self.language),
+            ShazamUrl.RELATED_SONGS.format(
+                language=self.language,
+                endpoint_country=self.endpoint_country,
+                limit=limit,
+                offset=offset,
+                track_id=track_id,
+            ),
             headers=self.headers(),
         )
 
-    async def search_artist(self, query: str, limit: int = 10) -> Dict[str, Any]:
+    async def search_artist(
+        self,
+        query: str,
+        limit: int = 10,
+        offset: int = 0,
+    ) -> Dict[str, Any]:
         """
         Search all artists by prefix or fullname
             :param query: Artist name or search prefix
             :param limit: Determines how many artists the maximum can be in the request.
                 Example: If 5 is specified, the query will return no more than 5 artists.
+            :param offset: A parameter that determines with which song to display the request.
+                The default is 0. If you want to skip the first few songs, set this parameter to
+                your own.
             :return: dict artists
         """
         return await self.request(
             "GET",
             ShazamUrl.SEARCH_ARTIST.format(
-                query,
-                limit,
                 language=self.language,
+                endpoint_country=self.endpoint_country,
+                limit=limit,
+                offset=offset,
+                query=query,
             ),
             headers=self.headers(),
         )
 
-    async def search_track(self, query: str, limit: int = 10) -> Dict[str, Any]:
+    async def search_track(self, query: str, limit: int = 10, offset: int = 0) -> Dict[str, Any]:
         """
         Search all tracks by prefix
             :param query: Track full title or prefix title
             :param limit: Determines how many songs the maximum can be in the request.
                 Example: If 5 is specified, the query will return no more than 5 songs.
+            :param offset: A parameter that determines with which song to display the request.
+                The default is 0. If you want to skip the first few songs, set this parameter to
+                your own.
             :return: dict songs
         """
         return await self.request(
             "GET",
             ShazamUrl.SEARCH_MUSIC.format(
-                query,
-                limit,
                 language=self.language,
+                endpoint_country=self.endpoint_country,
+                limit=limit,
+                offset=offset,
+                query=query,
             ),
             headers=self.headers(),
         )
 
     async def listening_counter(self, track_id: int) -> Dict[str, Any]:
         """
         Returns the total track listener counter.
@@ -341,14 +364,15 @@
             int(sig.number_samples / sig.sample_rate_hz * 1000),
             int(time.time() * 1000),
         )
 
         return await self.request(
             "POST",
             ShazamUrl.SEARCH_FROM_FILE.format(
-                str(uuid.uuid4()).upper(),
-                str(uuid.uuid4()).upper(),
                 language=self.language,
+                endpoint_country=self.endpoint_country,
+                uuid_1=str(uuid.uuid4()).upper(),
+                uuid_2=str(uuid.uuid4()).upper(),
             ),
             headers=self.headers(),
             json=data,
         )
```

### Comparing `shazamio-0.3.1.1/shazamio/client.py` & `shazamio-0.4.0.0/shazamio/client.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/converter.py` & `shazamio-0.4.0.0/shazamio/converter.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/enums.py` & `shazamio-0.4.0.0/shazamio/enums.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/factory.py` & `shazamio-0.4.0.0/shazamio/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         name_mapping={
             "photo_url": ("images", "coverarthq"),
             "ringtone": ("hub", "actions", 1, "uri"),
             "artist_id": ("artists", 0, "id"),
             "apple_music_url": ("hub", "options", 0, "actions", 0, "uri"),
             "spotify_url": ("hub", "providers", 0, "actions", 0, "uri"),
             "spotify_uri": ("hub", "providers", 0, "actions", 1, "uri"),
-            "_sections": "sections",
+            "sections": "sections",
         },
         skip_internal=True,
     )
 
     FACTORY_ARTIST_SCHEMA = Schema(
         name_mapping={
             "avatar": "avatar",
```

### Comparing `shazamio-0.3.1.1/shazamio/factory_misc.py` & `shazamio-0.4.0.0/shazamio/factory_misc.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/misc.py` & `shazamio-0.4.0.0/shazamio/misc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 from random import choice
 from shazamio.user_agent import USER_AGENTS
 
 
 class ShazamUrl:
     SEARCH_FROM_FILE = (
-        "https://amp.shazam.com/discovery/v5/en/GB/iphone/-/tag/{}/{"
-        "}?sync=true&webv3=true&sampling=true "
+        "https://amp.shazam.com/discovery/v5/{language}/{endpoint_country}/iphone/-/tag"
+        "/{uuid_1}/{uuid_2}?sync=true&webv3=true&sampling=true"
         "&connected=&shazamapiversion=v3&sharehub=true&hubv5minorversion=v5.1&hidelb=true&video=v3"
     )
     TOP_TRACKS_WORLD = (
-        "https://www.shazam.com/shazam/v3/en/GB/web/-/tracks/ip-global-chart"
-        "?pageSize={}&startFrom={}"
-    )
-    ARTIST_ABOUT = (
-        "https://www.shazam.com/discovery/v3/en/GB/web/artist/{" "}?shazamapiversion=v3&video=v3 "
-    )
-    ARTIST_TOP_TRACKS = (
-        "https://cdn.shazam.com/shazam/v3/en/GB/web/-/tracks/artisttoptracks_{}?startFrom={}"
-        "&pageSize={}&connected=&channel="
+        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
+        "/ip-global-chart?pageSize={limit}&startFrom={offset}"
     )
     ABOUT_TRACK = (
-        "https://www.shazam.com/discovery/v5/en/GB/web/-/track/{" "}?shazamapiversion=v3&video=v3 "
+        "https://www.shazam.com/discovery/v5/{language}/{endpoint_country}/web/-/track"
+        "/{track_id}?shazamapiversion=v3&video=v3 "
     )
     TOP_TRACKS_COUNTRY = (
-        "https://www.shazam.com/shazam/v3/en/GB/web/-/tracks/ip-country-chart-{}?pageSize={"
-        "}&startFrom={}"
+        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
+        "/ip-country-chart-{country_code}?pageSize={limit}&startFrom={offset}"
     )
     TOP_TRACKS_CITY = (
-        "https://www.shazam.com/shazam/v3/en/GB/web/-/tracks/ip-city-chart-{}?pageSize={"
-        "}&startFrom={}"
+        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
+        "/ip-city-chart-{city_id}?pageSize={limit}&startFrom={offset}"
     )
     CITY_IDS = "https://raw.githubusercontent.com/dotX12/dotX12/main/city.json"
     GENRE_WORLD = (
-        "https://www.shazam.com/shazam/v3/en/GB/web/-/tracks/genre-global-chart-{}?pageSize={"
-        "}&startFrom={}"
+        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
+        "/genre-global-chart-{genre}?pageSize={limit}&startFrom={offset}"
     )
     GENRE_COUNTRY = (
-        "https://www.shazam.com/shazam/v3/en/GB/web/-/tracks/genre-country-chart-{}-{}?pageSize={"
-        "}&startFrom={}"
+        "https://www.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
+        "/genre-country-chart-{country}-{genre}?pageSize={limit}&startFrom={offset}"
     )
     RELATED_SONGS = (
-        "https://cdn.shazam.com/shazam/v3/en/GB/web/-/tracks/track-similarities-id-{}"
-        "?startFrom={}&pageSize={}&connected=&channel="
+        "https://cdn.shazam.com/shazam/v3/{language}/{endpoint_country}/web/-/tracks"
+        "/track-similarities-id-{track_id}?startFrom={limit}&pageSize={offset}&connected=&channel="
     )
     SEARCH_ARTIST = (
-        "https://www.shazam.com/services/search/v4/en-US/RU/web/search?term={}"
-        "&offset=0&limit={}&types=artists"
+        "https://www.shazam.com/services/search/v4/{language}/{endpoint_country}/web"
+        "/search?term={query}&limit={limit}&offset={offset}&types=artists"
     )
     SEARCH_MUSIC = (
-        "https://www.shazam.com/services/search/v3/en/GB/web/search?query={}"
-        "&numResults={}&offset=0&types=songs"
+        "https://www.shazam.com/services/search/v3/{language}/{endpoint_country}/web"
+        "/search?query={query}&numResults={limit}&offset={offset}&types=songs"
     )
     LISTENING_COUNTER = "https://www.shazam.com/services/count/v2/web/track/{}"
 
-    SEARCH_ARTIST_V2 = "https://www.shazam.com/services/amapi/v1/catalog/{language}/artists/{}"
+    SEARCH_ARTIST_V2 = (
+        "https://www.shazam.com/services/amapi/v1/catalog/{endpoint_country}/artists/{artist_id}"
+    )
 
 
 class Request:
     TIME_ZONE = "Europe/Moscow"
 
     def __init__(self, language: str):
         self.language = language
```

### Comparing `shazamio-0.3.1.1/shazamio/schemas/artist/views/full_albums.py` & `shazamio-0.4.0.0/shazamio/schemas/artist/views/full_albums.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/schemas/artist/views/last_release.py` & `shazamio-0.4.0.0/shazamio/schemas/artist/views/last_release.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/schemas/artist/views/simular_artists.py` & `shazamio-0.4.0.0/shazamio/schemas/artist/views/simular_artists.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/schemas/artist/views/top_music.py` & `shazamio-0.4.0.0/shazamio/schemas/artist/views/top_music.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/schemas/artists.py` & `shazamio-0.4.0.0/shazamio/schemas/artists.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 
 from shazamio.schemas.artist.views.full_albums import FullAlbumsModel
 from shazamio.schemas.artist.views.last_release import LastReleaseModel
 from shazamio.schemas.artist.views.simular_artists import SimularArtist
 from shazamio.schemas.artist.views.top_music import TopMusicVideosView
+from shazamio.schemas.artist.views.top_song import TopSong
 from shazamio.schemas.attributes import ArtistAttribute
 from shazamio.schemas.enums import ArtistExtend
 from shazamio.schemas.enums import ArtistView
 from shazamio.schemas.errors import ErrorModel
 
 
 @dataclass
@@ -79,14 +80,15 @@
 
 
 class ArtistViews(BaseModel):
     top_music_videos: Optional[TopMusicVideosView] = Field(None, alias="top-music-videos")
     simular_artists: Optional[SimularArtist] = Field(None, alias="similar-artists")
     latest_release: Optional[LastReleaseModel] = Field(None, alias="latest-release")
     full_albums: Optional[FullAlbumsModel] = Field(None, alias="full-albums")
+    top_songs: Optional[TopSong] = Field(None, alias="top-songs")
 
 
 class ArtistV3(BaseModel):
     id: str
     type: str
     attributes: ArtistAttribute
     relationships: ArtistRelationships
```

### Comparing `shazamio-0.3.1.1/shazamio/schemas/models.py` & `shazamio-0.4.0.0/shazamio/schemas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     footer: str
     tab_name: str
     beacon_data: Optional[BeaconDataLyricsSection]
 
 
 @dataclass
 class VideoSection:
-    type: str
     tab_name: str
     youtube_url: str
+    type: str = "VIDEO"
 
 
 @dataclass
 class RelatedSection:
     type: str
     url: str
     tab_name: str
@@ -152,15 +152,15 @@
     photo_url: Optional[str] = field(init=False, default=None)
     spotify_uri_query: Optional[str] = None
     apple_music_url: Optional[str] = None
     ringtone: Optional[str] = None
     spotify_url: Optional[str] = field(default=None)
     spotify_uri: Optional[str] = field(default=None)
     youtube_link: Optional[str] = None
-    _sections: Optional[
+    sections: Optional[
         List[
             Union[
                 SongSection,
                 VideoSection,
                 RelatedSection,
                 ArtistSection,
                 LyricsSection,
@@ -181,15 +181,15 @@
         return url_deleted_query
 
     def __short_uri(self):
         if self.spotify_uri:
             return self.spotify_uri.split("spotify:search:")[1]
 
     def __youtube_link(self):
-        for i in self._sections:
+        for i in self.sections:
             if type(i) is VideoSection:
                 return i.youtube_url
 
 
 @dataclass
 class ResponseTrack:
     tag_id: Optional[UUID]
```

### Comparing `shazamio-0.3.1.1/shazamio/schemas/photos.py` & `shazamio-0.4.0.0/shazamio/schemas/photos.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/serializers.py` & `shazamio-0.4.0.0/shazamio/serializers.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/signature.py` & `shazamio-0.4.0.0/shazamio/signature.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/user_agent.py` & `shazamio-0.4.0.0/shazamio/user_agent.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/shazamio/utils.py` & `shazamio-0.4.0.0/shazamio/utils.py`

 * *Files identical despite different names*

### Comparing `shazamio-0.3.1.1/PKG-INFO` & `shazamio-0.4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shazamio
-Version: 0.3.1.1
+Version: 0.4.0.0
 Summary: Is a asynchronous framework from reverse engineered Shazam API written in Python 3.8+ with asyncio and aiohttp.
 Home-page: https://github.com/dotX12/ShazamIO
 License: MIT
 Keywords: python,shazam,music,recognize,api,async,asyncio,aiohttp,identification
 Author: dotX12
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -166,15 +166,15 @@
 import asyncio
 from shazamio import Shazam
 
 
 async def main():
     shazam = Shazam()
     track_id = 546891609
-    related = await shazam.related_tracks(track_id=track_id, limit=5, start_from=2)
+    related = await shazam.related_tracks(track_id=track_id, limit=5, offset=2)
     # ONLY №3, №4 SONG
     print(related)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
   ```
 </details>
@@ -233,27 +233,39 @@
 
 Get the top songs according to Shazam<br>
 <a href="https://www.shazam.com/artist/201896832/kizaru">https://www.shazam.com/artist/201896832/kizaru</a>
 
   ```python3
 import asyncio
 from shazamio import Shazam, Serialize
+from shazamio.schemas.artists import ArtistQuery
+from shazamio.schemas.enums import ArtistView
 
 
 async def main():
     shazam = Shazam()
-    artist_id = 201896832
-    top_three_artist_tracks = await shazam.artist_top_tracks(artist_id=artist_id, limit=3)
-    for track in top_three_artist_tracks['tracks']:
-        serialized_track = Serialize.track(data=track)
-        print(serialized_track)
+    artist_id = 1081606072
 
-loop = asyncio.get_event_loop()
+    about_artist = await shazam.artist_about(
+        artist_id,
+        query=ArtistQuery(
+            views=[
+                ArtistView.TOP_SONGS,
+            ],
+        ),
+    )
+    serialized = Serialize.artist_v2(about_artist)
+    for i in serialized.data[0].views.top_songs.data:
+        print(i.attributes.name)
+
+
+loop = asyncio.get_event_loop_policy().get_event_loop()
 loop.run_until_complete(main())
 
+
   ```
 </details>
 
 <details> 
 <summary>
 <i>🔝🎶🏙️ Top tracks in city</i>
 </summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shazamio Version: 0.3.1.1 Summary: Is a
+Metadata-Version: 2.1 Name: shazamio Version: 0.4.0.0 Summary: Is a
 asynchronous framework from reverse engineered Shazam API written in Python
 3.8+ with asyncio and aiohttp. Home-page: https://github.com/dotX12/ShazamIO
 License: MIT Keywords:
 python,shazam,music,recognize,api,async,asyncio,aiohttp,identification Author:
 dotX12 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -50,34 +50,37 @@
 track/559284007/rampampam shazam = Shazam() track_id = 559284007 count = await
 shazam.listening_counter(track_id=track_id) print(count) loop =
 asyncio.get_event_loop() loop.run_until_complete(main()) ```    ð¶ð¬
 Similar songs  Similar songs based song id
 https://www.shazam.com/track/546891609/2-phu%CC%81t-ho%CC%9Bn-kaiz-remix
 ```python3 import asyncio from shazamio import Shazam async def main(): shazam
 = Shazam() track_id = 546891609 related = await shazam.related_tracks
-(track_id=track_id, limit=5, start_from=2) # ONLY â3, â4 SONG print
-(related) loop = asyncio.get_event_loop() loop.run_until_complete(main()) ```
+(track_id=track_id, limit=5, offset=2) # ONLY â3, â4 SONG print(related)
+loop = asyncio.get_event_loop() loop.run_until_complete(main()) ```
 ðð¨âð¤ Search artists  Search all artists by prefix
 ```python3 import asyncio from shazamio import Shazam, Serialize async def main
 (): shazam = Shazam() artists = await shazam.search_artist(query='Lil',
 limit=5) for artist in artists['artists']['hits']: serialized =
 Serialize.artist(data=artist) print(serialized) loop = asyncio.get_event_loop()
 loop.run_until_complete(main()) ```    ðð¶ Search tracks  Search all
 tracks by prefix
 ```python3 import asyncio from shazamio import Shazam async def main(): shazam
 = Shazam() tracks = await shazam.search_track(query='Lil', limit=5) print
 (tracks) loop = asyncio.get_event_loop() loop.run_until_complete(main()) ```
 ðð¶ð¨âð¤ Top artist tracks  Get the top songs according to Shazam
 https://www.shazam.com/artist/201896832/kizaru ```python3 import asyncio from
-shazamio import Shazam, Serialize async def main(): shazam = Shazam() artist_id
-= 201896832 top_three_artist_tracks = await shazam.artist_top_tracks
-(artist_id=artist_id, limit=3) for track in top_three_artist_tracks['tracks']:
-serialized_track = Serialize.track(data=track) print(serialized_track) loop =
-asyncio.get_event_loop() loop.run_until_complete(main()) ```    ðð¶ðï¸
-Top tracks in city  Retrieving information from an artist profile
+shazamio import Shazam, Serialize from shazamio.schemas.artists import
+ArtistQuery from shazamio.schemas.enums import ArtistView async def main():
+shazam = Shazam() artist_id = 1081606072 about_artist = await
+shazam.artist_about( artist_id, query=ArtistQuery( views=
+[ ArtistView.TOP_SONGS, ], ), ) serialized = Serialize.artist_v2(about_artist)
+for i in serialized.data[0].views.top_songs.data: print(i.attributes.name) loop
+= asyncio.get_event_loop_policy().get_event_loop() loop.run_until_complete(main
+()) ```    ðð¶ðï¸ Top tracks in city  Retrieving information from an
+artist profile
 https://www.shazam.com/charts/top-50/russia/moscow ```python3 import asyncio
 from shazamio import Shazam, Serialize async def main(): shazam = Shazam()
 top_ten_moscow_tracks = await shazam.top_city_tracks(country_code='RU',
 city_name='Moscow', limit=10) print(top_ten_moscow_tracks) # ALL TRACKS DICT
 for track in top_ten_moscow_tracks['tracks']: serialized = Serialize.track
 (data=track) # SERIALIZE FROM DATACLASS FACTORY print(serialized) loop =
 asyncio.get_event_loop() loop.run_until_complete(main()) ```
```

