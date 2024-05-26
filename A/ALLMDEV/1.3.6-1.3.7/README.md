# Comparing `tmp/ALLMDEV-1.3.6-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 26891 bytes, number of entries: 22
+Zip file size: 29609 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
 -rw-rw-rw-  2.0 fat     4986 b- defN 24-May-11 17:03 ALLMDEV/azureagentapi.py
 -rw-rw-rw-  2.0 fat     3298 b- defN 24-May-11 16:47 ALLMDEV/azureagentchat.py
 -rw-rw-rw-  2.0 fat     2435 b- defN 24-May-11 16:47 ALLMDEV/azurecli.py
--rw-rw-rw-  2.0 fat    19203 b- defN 24-May-24 17:34 ALLMDEV/backend.py
+-rw-rw-rw-  2.0 fat    25481 b- defN 24-May-26 10:07 ALLMDEV/backend.py
+-rw-rw-rw-  2.0 fat     4952 b- defN 24-May-25 12:45 ALLMDEV/chat_history.py
 -rw-rw-rw-  2.0 fat     3221 b- defN 24-May-15 11:30 ALLMDEV/cli.py
 -rw-rw-rw-  2.0 fat    12685 b- defN 24-May-15 08:32 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
 -rw-rw-rw-  2.0 fat     2231 b- defN 24-May-22 04:35 ALLMDEV/serve.py
 -rw-rw-rw-  2.0 fat     1932 b- defN 24-May-15 12:35 ALLMDEV/studio.py
 -rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
 -rw-rw-rw-  2.0 fat     4530 b- defN 24-May-11 16:47 ALLMDEV/vertexagentapi.py
 -rw-rw-rw-  2.0 fat     2826 b- defN 24-May-14 10:42 ALLMDEV/vertexagentchat.py
 -rw-rw-rw-  2.0 fat     2126 b- defN 24-May-14 10:42 ALLMDEV/vertexcli.py
--rw-rw-rw-  2.0 fat     6093 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      591 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1698 b- defN 24-May-24 17:38 ALLMDEV-1.3.6.dist-info/RECORD
-22 files, 82015 bytes uncompressed, 24187 bytes compressed:  70.5%
+-rw-rw-rw-  2.0 fat     6093 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      591 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1778 b- defN 24-May-26 10:55 ALLMDEV-1.3.7.dist-info/RECORD
+23 files, 93325 bytes uncompressed, 26783 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: ALLMDEV/azurecli.py
 Comment: 
 
 Filename: ALLMDEV/backend.py
 Comment: 
 
+Filename: ALLMDEV/chat_history.py
+Comment: 
+
 Filename: ALLMDEV/cli.py
 Comment: 
 
 Filename: ALLMDEV/instruct.py
 Comment: 
 
 Filename: ALLMDEV/newagent.py
@@ -45,23 +48,23 @@
 
 Filename: ALLMDEV/vertexagentchat.py
 Comment: 
 
 Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.3.6.dist-info/METADATA
+Filename: ALLMDEV-1.3.7.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.3.6.dist-info/WHEEL
+Filename: ALLMDEV-1.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.3.6.dist-info/entry_points.txt
+Filename: ALLMDEV-1.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.6.dist-info/top_level.txt
+Filename: ALLMDEV-1.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.6.dist-info/RECORD
+Filename: ALLMDEV-1.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/backend.py

```diff
@@ -14,14 +14,16 @@
 from fastapi.responses import JSONResponse
 from langchain.document_loaders import CSVLoader, PDFMinerLoader, TextLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 import sqlite3
 import hashlib
+import re
+from datetime import datetime, timedelta
 
 
 
 app = FastAPI()
 
 
 
@@ -103,25 +105,29 @@
 def setup_database():
     conn = sqlite3.connect('user_database.db')
     cursor = conn.cursor()
 
     cursor.execute('''
     CREATE TABLE IF NOT EXISTS users (
         id INTEGER PRIMARY KEY AUTOINCREMENT,
-        username TEXT UNIQUE NOT NULL,
+        email TEXT UNIQUE NOT NULL,
         password TEXT NOT NULL,
         fullname TEXT NOT NULL           
     )
     ''')
 
     conn.commit()
     conn.close()
 
 config = load_config()
 
+def sanitize_email(email):
+    # Replace invalid characters with underscores
+    return re.sub(r'[^a-zA-Z0-9]', '_', email)
+
 @app.websocket("/model_config")
 async def websocket_model_config(websocket: WebSocket):
     await websocket.accept()
     try:
         while True:
             data = await websocket.receive_json()
             print("Received model config:", data)
@@ -308,14 +314,15 @@
             region=config["region"]
             model=config["model"]
             vertexai.init(project=projectid, location=region)
             multimodal_model = GenerativeModel(model_name=model)
             if agent == "None":
                 response = multimodal_model.generate_content(prompt)
                 await websocket.send_text(response.text)
+                await websocket.close()
             else:
 
                 persist_directory = os.path.join('db', agent)
                 embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
                 db = Chroma(embedding_function=embeddings, persist_directory=persist_directory)
 
                 docs = db.similarity_search(prompt, k=3)
@@ -368,14 +375,15 @@
                         {"role": "system", "content": "Assistant is a large language model trained by OpenAI."},
                         {"role": "user", "content": prompt}
                         
                     ]
                 )
                 for choice in response.choices:
                     await websocket.send_text(choice.message.content)
+                    await websocket.close()
             else:
                 persist_directory = os.path.join('db', agent)
                 if os.path.exists(persist_directory):
                     embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
                     db = Chroma(embedding_function=embeddings, persist_directory=persist_directory)
                     docs = db.similarity_search(prompt, k=3)
                     context = docs[0].page_content
@@ -484,27 +492,37 @@
         await websocket.close()
 
 @app.route('/signup', methods=['POST'])
 async def signup(request: Request):
     data = await request.json()
     print(data)
     fullname = data.get('fullname')
-    username = data.get('username')
+    email = data['email']
     password = data.get('password')
 
     hashed_password = hashlib.sha256(password.encode()).hexdigest()
 
     conn = sqlite3.connect('user_database.db')
     cursor = conn.cursor()
 
-    if '@' in username:
+    if '@' in email:
         try:
             cursor.execute('''
-            INSERT INTO users (username, password, fullname) VALUES (?, ?, ?)
-            ''', (username, hashed_password, fullname))
+            INSERT INTO users (email, password, fullname) VALUES (?, ?, ?)
+            ''', (email, hashed_password, fullname))
+
+            sanitized_table_name = sanitize_email(email)
+            cursor.execute(f'''
+            CREATE TABLE IF NOT EXISTS {sanitized_table_name} (
+                chat_id INTEGER PRIMARY KEY AUTOINCREMENT,
+                timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
+                messageheader TEXT,
+                chats TEXT                   
+            )
+        ''')
             conn.commit()
             response = {'message': 'User signed up successfully!'}
         except sqlite3.IntegrityError:
             response = {'message': 'Username already exists!'}
     else:
         response = {'message': 'Invalid email format.'}
     
@@ -513,39 +531,214 @@
     conn.close()
     return JSONResponse(content=response)
 
 # Route for user login
 @app.route('/login', methods=['POST'])
 async def login(request: Request):
     data = await request.json()
-    username = data.get('username')
-    password = data.get('password')
-
-    if not username or not password:
-        raise HTTPException(status_code=400, detail="Username and password required")
+    email = data['email']
+    password = data['password']
 
     hashed_password = hashlib.sha256(password.encode()).hexdigest()
 
     conn = sqlite3.connect('user_database.db')
     cursor = conn.cursor()
 
     cursor.execute('''
-    SELECT * FROM users WHERE username = ? AND password = ?
-    ''', (username, hashed_password))
+    SELECT id, fullname FROM users WHERE email = ? AND password = ?
+    ''', (email, hashed_password))
 
     user = cursor.fetchone()
 
     if user:
-        response = {'message': 'Login successful!'}
+        print(user)
+        user_id = user[0]
+        fullname = user[1]
+        print(fullname, user_id)
+        response = {'message': f"Welcome, {fullname}!","status": True, "user_id": user_id}
     else:
         response = {'message': 'Invalid username or password.'}
 
     conn.close()
     return JSONResponse(content=response)
 
+@app.post('/newchat')
+async def update_chat_history(request: Request):
+    data = await request.json()
+    print(data)
+    user_email = data['userEmail']
+    message_header = data['messageheader']
+    chats = data['chats']
+    
+    # Convert the chats array to a JSON string
+    chats_json = json.dumps(chats)
+
+    # Connect to the database
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    try:
+        # Execute query to insert data into the specified user's table
+        cursor.execute(f'''
+            INSERT INTO {user_email} (messageheader, chats)
+            VALUES (?, ?)
+        ''', (message_header, chats_json))
+
+        cursor.execute(f'''
+            SELECT chat_id FROM {user_email}
+            WHERE messageheader = ?
+        ''', (message_header,))
+        
+        # Fetch the chat_id
+        chat_id = cursor.fetchone()[0]
+
+        # Commit the transaction
+        conn.commit()
+
+        # Close the database connection
+        conn.close()
+
+        return JSONResponse(content={'message': 'Chat history updated successfully.', 'chat_id': chat_id})
+    except Exception as e:
+        # Rollback changes if an error occurs
+        conn.rollback()
+        conn.close()
+        raise HTTPException(status_code=500, detail=f'Error updating chat history: {str(e)}')
+    
+
+@app.post('/fetchchat')
+async def fetch_chat_history(request: Request):
+    data = await request.json()
+    print(data)
+    user_email = data['userEmail']
+    chat_id = data['chat_id']
+
+    # Connect to the database
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    try:
+        # Execute query to fetch chat history based on userEmail and chat_id
+        cursor.execute(f'''
+            SELECT chats FROM {user_email}
+            WHERE chat_id = ?
+        ''', (chat_id,))
+        
+        # Fetch the chat history
+        chat_history = cursor.fetchone()
+
+        if chat_history:
+            # Parse the chat history from JSON
+            chat_history_json = json.loads(chat_history[0])
+            return JSONResponse(content={'chat': chat_history_json})
+        else:
+            raise HTTPException(status_code=404, detail='Chat history not found.')
+    except Exception as e:
+        raise HTTPException(status_code=500, detail=f'Error fetching chat history: {str(e)}')
+    finally:
+        # Close the database connection
+        conn.close()
+
+@app.post('/updatechat')
+async def update_chat_history(request: Request):
+    data = await request.json()
+    user_email = data['userEmail']
+    chat_id = data['chat_id']
+    updated_chats = data['chats']
+    
+    # Convert the updated chats array to a JSON string
+    updated_chats_json = json.dumps(updated_chats)
+
+    # Connect to the database
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    try:
+        # Execute query to update the chat data for the specified chat_id
+        cursor.execute(f'''
+            UPDATE {user_email}
+            SET chats = ?
+            WHERE chat_id = ?
+        ''', (updated_chats_json, chat_id))
+
+        # Check if any rows were affected
+        if cursor.rowcount == 0:
+            raise HTTPException(status_code=404, detail="Chat not found.")
+        
+        # Commit the transaction
+        conn.commit()
+
+        return JSONResponse(content={'message': 'Chat history updated successfully.'})
+    except Exception as e:
+        raise HTTPException(status_code=500, detail=f'Error updating chat history: {str(e)}')
+    finally:
+        # Close the database connection
+        conn.close()
+
+def get_start_of_day(date):
+    return date.replace(hour=0, minute=0, second=0, microsecond=0)
+
+def get_date_x_days_ago(days):
+    return get_start_of_day(datetime.now() - timedelta(days=days))
+
+@app.post('/fetchchatsidebar')
+async def fetch_chat_sidebar(request: Request):
+    data = await request.json()
+    print(data)
+    user_email = data.get('userEmail')
+
+    if not user_email:
+        raise HTTPException(status_code=400, detail='userEmail is required')
+
+    email_safe = user_email.replace('.', '_').replace('@', '_')
+    today_start = get_start_of_day(datetime.now())
+    seven_days_ago = get_date_x_days_ago(7)
+
+    conn = sqlite3.connect('user_database.db')
+    cursor = conn.cursor()
+
+    try:
+        cursor.execute(f'''
+            SELECT chat_id, messageheader, timestamp
+            FROM {email_safe}
+        ''')
+
+        chats = cursor.fetchall()
+
+        today_chats = []
+        past_seven_days_chats = []
+
+        for chat in chats:
+            chat_id, message_header, timestamp = chat
+            chat_date = datetime.fromisoformat(timestamp)
+
+            if chat_date >= today_start:
+                today_chats.append({
+                    'chat_id': chat_id,
+                    'message_header': message_header,
+                    'timestamp': timestamp
+                })
+            elif chat_date >= seven_days_ago:
+                past_seven_days_chats.append({
+                    'chat_id': chat_id,
+                    'message_header': message_header,
+                    'timestamp': timestamp
+                })
+
+        print(today_chats, past_seven_days_chats)
+        return JSONResponse(content={
+            'today': today_chats,
+            'past_seven': past_seven_days_chats
+        })
+
+    except Exception as e:
+        raise HTTPException(status_code=500, detail=f'Error fetching chat sidebar: {str(e)}')
+    finally:
+        conn.close()
+
 def main():
     import uvicorn
     setup_database()
     uvicorn.run(app, host="0.0.0.0", port=8000)
 
 if __name__ == "__main__":
     main()
```

## Comparing `ALLMDEV-1.3.6.dist-info/METADATA` & `ALLMDEV-1.3.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.3.6
+Version: 1.3.7
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
```

## Comparing `ALLMDEV-1.3.6.dist-info/entry_points.txt` & `ALLMDEV-1.3.7.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ALLMDEV-1.3.6.dist-info/RECORD` & `ALLMDEV-1.3.7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
 ALLMDEV/agentapi.py,sha256=vnkpCaviW0w5EQTE99els4Nb8QABv0TgNoP2FdFsWVQ,3706
 ALLMDEV/agentchat.py,sha256=UHLn4mVEBz6C77G8aaf3DWrzuVPfA-PCEp6uFZpcGyM,3440
 ALLMDEV/azureagentapi.py,sha256=dzMwkJHfRBqRxYAwpe_aQRgASqnsNBaEzT9jsc791QQ,4986
 ALLMDEV/azureagentchat.py,sha256=6L9m2B6dfe9LUWdd_Vj6_TT1n1GBXxVvqOeA-yTuV_Q,3298
 ALLMDEV/azurecli.py,sha256=nLoSVPpxWwIJWhiddB0_qzNw53hrAE6ijK0diDlaGYs,2435
-ALLMDEV/backend.py,sha256=b2GcDlcgeyMbwMcyLtrYGCTPS8v68NAylj9LMXqBdt0,19203
+ALLMDEV/backend.py,sha256=owOM8c2NBz2Z4sxzqBCd0hbNJq79nQ1aZrlETzco0Jc,25481
+ALLMDEV/chat_history.py,sha256=Et8kDK4RKdIr-v4CoYdvd5yb37GxTHpu4U1gHw5C2GY,4952
 ALLMDEV/cli.py,sha256=13o2i7g_DtOyP8N8x7QdMr8iUGr4raJX26NJ9oqpgNw,3221
 ALLMDEV/instruct.py,sha256=-3ybhrmAwgLy_MptpJHhFnbQq1NcT4DHeMV2-46Tzl8,12685
 ALLMDEV/newagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/serve.py,sha256=RUKwji_795izII7XlYku1KUK6bvgR_SYBB9N34GwqUA,2231
 ALLMDEV/studio.py,sha256=LlrIEWcs-o8cIjnprJVijR8cNxrOsnFvl9AgTrk43iw,1932
 ALLMDEV/test.py,sha256=CxP_WW9ZXEiLCJh_9MLdieFU-yfNMwWlXrcrs7gtXx8,683
 ALLMDEV/updateagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/vertexagentapi.py,sha256=fPbLJoy8Wirh7wPc31EzlgLSqfF2e4PkEwYCO9h4yqk,4530
 ALLMDEV/vertexagentchat.py,sha256=dYvJ2_teBGeEN3TTrXq4pSulYJW5kmNPKFa9xg9ec9s,2826
 ALLMDEV/vertexcli.py,sha256=-5BgOKO7oMsjcsJRluAM0ivWllzpBpWmVQIzHbq_Xrk,2126
-ALLMDEV-1.3.6.dist-info/METADATA,sha256=QA5iZEbmyTb4ZhlkxjmrD8iQaTthyZp1ju4eAqS_57Y,6093
-ALLMDEV-1.3.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.3.6.dist-info/entry_points.txt,sha256=u71vTXywZkZgH8fa1luPKfAsQCbItzqCHI6DgWpJGH4,591
-ALLMDEV-1.3.6.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.3.6.dist-info/RECORD,,
+ALLMDEV-1.3.7.dist-info/METADATA,sha256=rNUB4sPvqmJt5ZVgK3pTXFbl0xIubg3FDBLKAyU0c7w,6093
+ALLMDEV-1.3.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.3.7.dist-info/entry_points.txt,sha256=u71vTXywZkZgH8fa1luPKfAsQCbItzqCHI6DgWpJGH4,591
+ALLMDEV-1.3.7.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.3.7.dist-info/RECORD,,
```

