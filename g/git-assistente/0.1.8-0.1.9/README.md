# Comparing `tmp/git_assistente-0.1.8.tar.gz` & `tmp/git_assistente-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_assistente-0.1.8.tar", last modified: Mon Dec 18 16:56:32 2023, max compression
+gzip compressed data, was "git_assistente-0.1.9.tar", last modified: Sun May 26 16:58:40 2024, max compression
```

## Comparing `git_assistente-0.1.8.tar` & `git_assistente-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 16:56:32.085323 git_assistente-0.1.8/
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1089 2023-12-10 20:42:35.000000 git_assistente-0.1.8/LICENSE
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1230 2023-12-18 16:56:32.085323 git_assistente-0.1.8/PKG-INFO
--rw-r--r--   0 carlos    (1000) carlos    (1000)      934 2023-12-13 18:34:55.000000 git_assistente-0.1.8/README.md
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 16:56:32.075323 git_assistente-0.1.8/git_assistente/
--rw-r--r--   0 carlos    (1000) carlos    (1000)       22 2023-12-10 23:10:44.000000 git_assistente-0.1.8/git_assistente/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     8301 2023-12-18 16:55:20.000000 git_assistente-0.1.8/git_assistente/__main__.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 16:56:32.085323 git_assistente-0.1.8/git_assistente/core/
--rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2023-12-11 20:10:37.000000 git_assistente-0.1.8/git_assistente/core/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      569 2023-12-10 18:24:44.000000 git_assistente-0.1.8/git_assistente/core/check_response.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      252 2023-12-12 16:10:40.000000 git_assistente-0.1.8/git_assistente/core/clear.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      331 2023-12-10 15:23:04.000000 git_assistente-0.1.8/git_assistente/core/cmd.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      132 2023-12-10 15:23:04.000000 git_assistente-0.1.8/git_assistente/core/get_repository_name.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      205 2023-12-12 13:45:53.000000 git_assistente-0.1.8/git_assistente/core/typewriter.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 16:56:32.085323 git_assistente-0.1.8/git_assistente/utils/
--rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2023-12-11 20:10:58.000000 git_assistente-0.1.8/git_assistente/utils/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1548 2023-12-18 16:56:16.000000 git_assistente-0.1.8/git_assistente/utils/banner.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 16:56:32.075323 git_assistente-0.1.8/git_assistente.egg-info/
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1230 2023-12-18 16:56:32.000000 git_assistente-0.1.8/git_assistente.egg-info/PKG-INFO
--rw-r--r--   0 carlos    (1000) carlos    (1000)      577 2023-12-18 16:56:32.000000 git_assistente-0.1.8/git_assistente.egg-info/SOURCES.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)        1 2023-12-18 16:56:32.000000 git_assistente-0.1.8/git_assistente.egg-info/dependency_links.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       65 2023-12-18 16:56:32.000000 git_assistente-0.1.8/git_assistente.egg-info/entry_points.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       18 2023-12-18 16:56:32.000000 git_assistente-0.1.8/git_assistente.egg-info/requires.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       15 2023-12-18 16:56:32.000000 git_assistente-0.1.8/git_assistente.egg-info/top_level.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       38 2023-12-18 16:56:32.085323 git_assistente-0.1.8/setup.cfg
--rw-r--r--   0 carlos    (1000) carlos    (1000)      613 2023-12-18 16:56:13.000000 git_assistente-0.1.8/setup.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-05-26 16:58:40.514366 git_assistente-0.1.9/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1089 2024-01-05 13:08:49.000000 git_assistente-0.1.9/LICENSE
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1230 2024-05-26 16:58:40.514366 git_assistente-0.1.9/PKG-INFO
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      934 2024-01-05 13:08:49.000000 git_assistente-0.1.9/README.md
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-05-26 16:58:40.514366 git_assistente-0.1.9/git_assistente/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       22 2024-01-05 13:08:49.000000 git_assistente-0.1.9/git_assistente/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     7001 2024-05-12 19:37:08.000000 git_assistente-0.1.9/git_assistente/__main__.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-05-26 16:58:40.514366 git_assistente-0.1.9/git_assistente/core/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2024-01-05 13:08:49.000000 git_assistente-0.1.9/git_assistente/core/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      569 2024-01-05 13:08:49.000000 git_assistente-0.1.9/git_assistente/core/check_response.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      252 2024-05-12 19:29:24.000000 git_assistente-0.1.9/git_assistente/core/clear.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      456 2024-05-12 18:03:29.000000 git_assistente-0.1.9/git_assistente/core/cmd.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      132 2024-01-05 13:08:49.000000 git_assistente-0.1.9/git_assistente/core/get_repository_name.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      205 2024-01-05 13:08:49.000000 git_assistente-0.1.9/git_assistente/core/typewriter.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-05-26 16:58:40.514366 git_assistente-0.1.9/git_assistente/utils/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2024-01-05 13:08:49.000000 git_assistente-0.1.9/git_assistente/utils/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1594 2024-05-12 19:22:00.000000 git_assistente-0.1.9/git_assistente/utils/banner.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-05-26 16:58:40.514366 git_assistente-0.1.9/git_assistente.egg-info/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1230 2024-05-26 16:58:40.000000 git_assistente-0.1.9/git_assistente.egg-info/PKG-INFO
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      577 2024-05-26 16:58:40.000000 git_assistente-0.1.9/git_assistente.egg-info/SOURCES.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        1 2024-05-26 16:58:40.000000 git_assistente-0.1.9/git_assistente.egg-info/dependency_links.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       65 2024-05-26 16:58:40.000000 git_assistente-0.1.9/git_assistente.egg-info/entry_points.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       18 2024-05-26 16:58:40.000000 git_assistente-0.1.9/git_assistente.egg-info/requires.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       15 2024-05-26 16:58:40.000000 git_assistente-0.1.9/git_assistente.egg-info/top_level.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       38 2024-05-26 16:58:40.514366 git_assistente-0.1.9/setup.cfg
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      613 2024-05-12 19:38:26.000000 git_assistente-0.1.9/setup.py
```

### Comparing `git_assistente-0.1.8/LICENSE` & `git_assistente-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `git_assistente-0.1.8/PKG-INFO` & `git_assistente-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_assistente
-Version: 0.1.8
+Version: 0.1.9
 Summary: Um assistente do Git para subir projetos no GitHub
 Home-page: UNKNOWN
 Author: CarlosAllberto
 Author-email: dasilvacarlosalberto344@gmail.com
 License: MIT License
 Keywords: git assistente
 Platform: UNKNOWN
```

### Comparing `git_assistente-0.1.8/README.md` & `git_assistente-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `git_assistente-0.1.8/git_assistente/__main__.py` & `git_assistente-0.1.9/git_assistente/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,225 +1,204 @@
 #!/usr/bin/python
 
+import requests 
 from sys import exit
-from git_assistente.core.cmd import cmd
+from colorama import Fore, Style
+
+from git_assistente.core.cmd import cmd, cmd_print
 from git_assistente.core.get_repository_name import get_repository_name
 from git_assistente.core.typewriter import typewriter
 from git_assistente.core.check_response import check_response
 from git_assistente.core.clear import clear
 from git_assistente.utils.banner import banner
-from colorama import Fore, Style
-from os import system
-import requests 
 
 red = Fore.RED
 green = Fore.GREEN
-reset = Fore.RESET
 dim = Style.DIM
-reset_all = Style.RESET_ALL
-
-class git_assistente:
-    def __init__(self):
-        system("clear")
-        banner()
-        git_config = {}
-
-        self.first = ""
-        
-        try:
-            result_cmd = str(cmd("git config --list").stdout, encoding="utf-8").split()
-            for line in result_cmd:
-                line = line.split("=")
-                git_config[line[0]] = line[1]
-            self.git_config = git_config
-        except:
-            pass
-
-        try:
-            self.name = git_config['user.name']
-            self.email = git_config['user.email']
-        except:
-            self.first = True
-    
-        cmd("git config --global credential.helper store")
-        cmd("git config --global pull.rebase true")
-        print(f"{green}[+] Configuraçãoes de ajuda feitas{reset}")
-
+reset = Fore.RESET
 
+message_token = f"""
+[INFO]: Faça a criação do seu token em https://github.com/settings/tokens\n
+{dim}[DICA]: Você pode seguir as etapas abaixo: 
+0 - Abra o link acima
+1 - Clique em \"Generate new token\"
+2 - Escolha a opção classic
+3 - Marque todas as caixinhas
+4 - Gere seu token.
+5 - Guarde o token. O git vai pedir nestante.{reset}\n
+[OBS]: o token sera salvo e não sera pedido novamente.
+"""
 
-    # verifica se é primeira vez usando o assistente
-    def verify_first(self):
-        if self.first:
-            typewriter("Olá, sou seu novo assistente do Git. \ncomo parece ser sua primeira vez usando o Git preciso saber quem é você.\n")
-            name = str(input("Me diga seu Username usado no GitHub: "))
-            cmd(f"git config --global user.name \"{name}\"")
-            print(f"{green}[+] Username cadastrado com sucesso{reset}")
-            clear()
-            typewriter(f"Prazer em te conhecer, {name}")
-            clear()
-            email = str(input("Agora Digite seu Email: "))
-            cmd(f"git config --global user.email \"{email}\"")
-            print(f"{green}[+] Email cadastrado com sucesso{reset}")
-            clear()
-            self.name = name
+class git_assistente:
+  def __init__(self):
+    banner()
 
+    git_config = {}
+    self.is_first = False
 
+    try:
+      result = str(cmd("git config --list").stdout, encoding="utf-8").split()
+      for line in result:
+        line = line.split("=")
+        git_config[line[0]] = line[1]
+
+      self.name = git_config['user.name']
+    except:
+      self.is_first = True
+
+    cmd("git config --global credential.helper store")
+    cmd("git config --global pull.rebase true")
+
+
+  # boas vindas
+  def first(self):
+    if self.is_first:
+      typewriter("Olá, sou seu novo assistente do Git. \ncomo parece ser sua primeira vez usando o Git preciso saber quem é você.\n")
+      name = str(input("Me diga seu Username usado no GitHub: "))
+      cmd_print(f"git config --global user.name \"{name}\"")
+      print(f"{green}[+] Username cadastrado com sucesso{reset}")
+      clear()
+      typewriter(f"Prazer em te conhecer, {name}")
+      clear()
+      email = str(input("Agora Digite seu Email usado no GitHub: "))
+      cmd_print(f"git config --global user.email \"{email}\"")
+      print(f"{green}[+] Email cadastrado com sucesso{reset}")
+      clear()
+      self.name = name
+
+
+  # verifica conexão com repositório
+  def verify_repository_connect(self):
+    try: 
+      result = str(cmd_print("git remote -v").stdout, encoding="utf-8")
+      if "not a git repository" in result:
+        typewriter("Seu projeto ainda não foi conectado à um repositório no GitHub.\n")
+        return True
+    except: 
+      exit("Erro ao verificar conexão com repositório.")
+
+  
+  # verifica se o repositório existe no GitHub
+  def vefify_exists_repository(self):
+    try:
+      repositories = requests.get(f"https://api.github.com/users/{self.name}/repos").json()
+      repository_name = [repo["name"] for repo in repositories]
+      repository = get_repository_name()
+      if repository in repository_name:
+        return True
+      
+      typewriter(f"Para fazermos a ligação da pasta com o GitHub é preciso que já exista um repósitorio VÁZIO com o nome {repository}\n no seu GitHub.")
+      typewriter("Faça a criação do repositório e me chame novamente.")
+      exit()
+    except:
+      exit("Não foi possivel listar os repositorios. \nVerifique a conexão com a sua internet.")
+
+
+  # faz a conexão com o repositório no GitHub
+  def repository_connect(self):
+    typewriter("Vamos fazer a conexão agora\n")
+    repository = get_repository_name()
+    try:
+      cmd_print("git init")
+      cmd_print(f"git remote add origin https://github.com/{self.name}/{repository}.git")
+      cmd_print("git branch -M main")
+      print(f"{green}[+] Conexão feita com sucesso.{reset}")
+    except:
+      exit("Erro ao fazer conexão com repositório.")
+
+
+  # verifica se tem alguma coisa para dar commit no seu projeto
+  def verify_commit(self):
+    try:
+      result = str(cmd_print("git fetch && git status -uno").stdout, encoding="utf-8")
+      if "nothing to commit" in result:
+        return print("Seu projeto não tem nenhuma atualização para dar commit.")
+      return True
+    except:
+      exit("Erro ao verificar se tem alguma coisa para dar commit.")
+
+
+  # adiciona commit no projeto
+  def commit(self):
+    try: 
+      cmd_print("git add .")
+      print("Commit é um breve resumo das atualizações feitas no repositório. \nExemplo: [editei o arquivo.py, excluir o arquivo teste.py, refatoração, alteração no estilo]\nCaso escolha não passar um commit sera utilizado um commit padrão.\n")
+      if check_response("Deseja adicionar um commit?"):
+        commit = str(input("Digite seu commit: "))
+        return cmd_print(f"git commit -m \"{commit}\"") 
+      cmd_print("git commit -m \"Add files via GitAssistente\"")
+    except:
+      exit("Erro ao dar commit no projeto.")
+
+
+  # verifica se o repositório tem alguma atualização pedente
+  def verify_pull(self):
+    try:        
+      result = str(cmd_print("git fetch && git status").stdout, encoding="utf-8")
+      
+      if "git pull" in result:
+        print("O projeto tem atualizaçãoes mais recentes no GitHub que devemos trazer para a sua máquina antes de subir o projeto.")
+        print("Isso pode fazer com que algumas coisas possam ser sobreescritas.\n")
+        if check_response("Deseja trazer as atualizações para sua máquina?"):
+          return True
+        exit("Não é possivel subir as atualizações para o GitHub sem antes trazer as modificações.")
+     
+    except:
+        exit("Erro ao verificar atualização no GitHub.")
+
+
+  # puxa as coisas do repositório do GitHub para sua máquina
+  def pull(self):
+    try:
+      result = str(cmd_print("git pull origin main").stdout, encoding="utf-8")
+      if "Successfully rebased and updated" in result:
+        print(f"{green}[+] Modificações do GitHub puxadas para a sua maquina.{reset}")
+    except:
+      exit("Erro ao trazer atualizaçãoes do GitHub para o sua máquina.")
+  
+  
+  # sobe o projeto
+  def push(self):
+    try:
+      if self.is_first:
+        print(message_token)
+        clear()
+
+      if self.verify_pull():
+        self.pull()
+      
+      result = str(cmd_print("git push origin main").stdout, encoding="utf-8")
+
+      repository_name = get_repository_name()
+
+      if f"To https://github.com/{self.name}/{repository_name}" in result:
+        return print(f"{green}[+] Projeto subiu no GitHub com sucesso!{reset}")
+      
+      if "Everything up-to-date" in result:
+        return print("Seu projeto não tem nenhuma atualização para subir.")
+
+      print("Nâo foi possivel subir o projeto no GitHub.")
+    except Exception as error:
+      print(error)
+      exit("Erro ao subir o projeto no GitHub.")
+  
+  
+  # executa a ferramenta na ordem certa
+  def run(self):
+    self.first()
+    
+    if self.verify_repository_connect():
+      if self.vefify_exists_repository():
+        self.repository_connect()
 
-    # verifica conexão com repositório
-    def verify_repository_connect(self):
-        try: 
-            result_cmd = str(cmd("git remote -v").stdout, encoding="utf-8")
-            if "not a git repository" in result_cmd:
-                typewriter("Seu projeto ainda não foi conectado à um repositório no GitHub.\n")
-                return True
-        except: 
-            exit("Erro ao verificar conexão com repositório.")
-        
+    if self.verify_commit():
+      self.commit()
 
-    
-    # verifica se o repositório existe no GitHub
-    def vefify_exists_repository(self):
-        try:
-            repositories = requests.get(f"https://api.github.com/users/{self.name}/repos").json()
-            repository_name = [repo["name"] for repo in repositories]
-            repository = get_repository_name()
-            if repository in repository_name:
-                return True
-            
-            typewriter(f"Para fazermos a ligação da pasta com o GitHub é preciso que já exista um repósitorio VÁZIO com o nome {repository}\n no seu GitHub.")
-            typewriter("Faça a criação do repositório e me chame novamente.")
-            exit()
-        except:
-            exit("Não foi possivel listar os repositorios. \nVerifique a conexão com a sua internet.")
-
-
-
-    # faz a conexão com o repositório no GitHub
-    def repository_connect(self):
-        typewriter("Vamos fazer a conexão agora\n")
-        repository = get_repository_name()
-        try:
-            cmd("git init")
-            cmd(f"git remote add origin https://github.com/{self.name}/{repository}.git")
-            cmd("git branch -M main")
-            print(f"{green}[+] Conexão feita com sucesso.{reset}")
-        except:
-            exit("Erro ao fazer conexão com repositório.")
-
-
-
-    # verifica se tem alguma coisa para dar commit no seu projeto
-    def verify_commit(self):
-        try:
-            cmd_result = str(cmd("git status").stdout, encoding="utf-8")
-            if "nothing to commit" in cmd_result:
-                return print("Seu projeto não tem nenhuma atualização para dar commit.")
-            return True
-        except:
-            exit("Erro ao verificar se tem alguma coisa para dar commit.")
-
-
-
-    # adiciona commit no projeto
-    def commit(self):
-        try: 
-            cmd("git add .")
-            print("Commit é um breve resumo das atualizações feitas no repositório. \nExemplo: [editei o arquivo.py, excluir o arquivo teste.py, refatoração, alteração no estilo]\nCaso escolha não passar um commit sera utilizado um commit padrão.\n")
-            if check_response("Deseja adicionar um commit?"):
-                commit = str(input("Digite seu commit: "))
-                return cmd(f"git commit -m \"{commit}\"") 
-            cmd("git commit -m \"Add files via GitAssistente\"")
-        except:
-            exit("Erro ao dar commit no projeto.")
-
-
-
-    # verifica se o repositório tem alguma atualização pedente
-    def verify_pull(self, cmd_result=""):
-        try:
-            if cmd_result == "":
-                cmd("git fetch")
-                cmd_result = str(cmd("git status").stdout, encoding="utf-8")
-            
-            if "git pull" in cmd_result:
-                print("O projeto tem atualizaçãoes mais recentes no GitHub que devemos trazer para a sua máquina.")
-                print("Isso pode fazer com que algumas coisas possam ser sobreescritas.\n")
-                if check_response("Deseja trazer as atualizações para sua máquina?"):
-                    return True
-                exit("Não é possivel subir as atualizações para o GitHub sem antes trazer as modificações.")
-        except:
-            exit("Erro ao verificar atualização no GitHub.")
-
-
-
-    # puxa as coisas do repositório do GitHub para sua máquina
-    def pull(self):
-        try:
-            cmd_result = str(cmd("git pull origin main").stdout, encoding="utf-8")
-            if "Already up to date." in cmd_result:
-                return print("Nada para atualizar.")
-            if "Successfully rebased and updated" in cmd_result:
-                print(f"{green}[+] Modificações do GitHub puxadas para a sua maquina.{reset}")
-        except:
-            exit("Erro ao trazer atualizaçãoes do GitHub para o sua máquina.")
-    
-    
-    
-    # sobe o projeto
-    def push(self):
-        try:
-            if self.first:
-                print("[INFO]: Faça a criação do seu token em https://github.com/settings/tokens\n")
-                print(f"""{dim}[DICA]: Você pode seguir as etapas abaixo: 
-                0 - Abra o link acima
-                1 - Clique em \"Generate new token\"
-                2 - Escolha a opção classic
-                3 - Marque todas as caixinhas
-                4 - Gere seu token.
-                5 - Guarde o token. O git vai pedir nestante.{reset_all}\n
-                """)
-                print("[OBS]: o token sera salvo e não sera pedido novamente.\n")
-                clear()
-
-            cmd_result = str(cmd("git push origin main").stdout, encoding="utf-8")
-
-            repository_name = get_repository_name()
-
-            if f"To https://github.com/{self.name}/{repository_name}.git" in cmd_result:
-                return print(f"{green}[+] Projeto subiu no GitHub com sucesso!{reset}")
-            
-            if "Everything up-to-date" in cmd_result:
-                return print("Seu projeto não tem nenhuma atualização para subir.")
-            
-            if self.verify_pull(cmd_result):
-                self.pull()
-                self.push()
-
-            print("Nâo foi possivel subir o projeto no GitHub.")
-        except:
-            exit("Erro ao subir o projeto no GitHub.")
-    
-    
-
-    # executa a ferramenta na ordem certa
-    def run(self):
-        self.verify_first()
+      if self.verify_pull():
+        self.pull()
         
-        if self.verify_repository_connect():
-            if self.vefify_exists_repository():
-                self.repository_connect()
-
-        if self.verify_commit():
-            self.commit()
-
-            if self.verify_pull():
-                self.pull()
-            
-        self.push()      
-
-def main():
-    git_assistente().run()  
+    self.push()       
 
 if __name__ == "__main__":
-    main()
+  git_assistente().run()  
 
 typewriter("\nAté a próxima.\n")
```

### Comparing `git_assistente-0.1.8/git_assistente/core/check_response.py` & `git_assistente-0.1.9/git_assistente/core/check_response.py`

 * *Files identical despite different names*

### Comparing `git_assistente-0.1.8/git_assistente/utils/banner.py` & `git_assistente-0.1.9/git_assistente/utils/banner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from colorama import Fore
 from dankware import align
+from os import system
 
 art = """
 ⠀⠀⠀⣤⣤⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣤⣤⠀⠀⠀
 ⠀⠀⢸⣿⣿⣿⣿⣦⣀⣀⣤⣤⣤⣤⣤⣤⣄⣠⣶⣿⣿⣿⣿⡇⠀⠀
 ⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡇⠀⠀
 ⠀⠀⣤⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣦⠀⠀
 ⠀⣼⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣧⠀
@@ -12,16 +13,17 @@
 ⠘⣿⣿⣿⡇⠀⢠⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⡄⠀⢸⣿⣿⣿⠃
 ⠀⢿⣿⣿⡇⠀⠀⠛⠟⠀⠀⠀⠀⠀⠀⠀⠀⠻⠛⠀⠀⢸⣿⣿⡟⠀
 ⠀⠀⠻⣿⣿⣆⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣾⣿⠟⠀⠀
 ⠀⠀⠀⠀⠙⠛⠿⣷⣶⣤⣤⣤⣤⣤⣤⣤⣤⣴⣶⠿⠛⠋⠀⠀⠀⠀
 """
 
 def banner():
-    print(align(f"{Fore.BLUE}{art}{Fore.RESET}\n"))
-    print(align(f"{Fore.YELLOW}[-]              Version: 0.1.8              [-]{Fore.RESET}"))
-    print(align(f"{Fore.YELLOW}[-]          Author: CarlosAllberto          [-]{Fore.RESET}"))
-    print(align(f"{Fore.YELLOW}[-]   GitHub: www.github.com/CarlosAllberto  [-]{Fore.RESET}"))
-    print(align(f"[*]            *****************             [*]"))
-    print(align(f"Projeto criado com o a intuito de ajudar\n iniciantes e profissionais a subir projetos \nno GitHub de forma super rápida.\n"))
+    system("clear")
+    print(f"{Fore.GREEN}{art}{Fore.RESET}\n")
+    # print(align(f"{Fore.YELLOW}[-]              Version: 0.1.8              [-]{Fore.RESET}"))
+    # print(align(f"{Fore.YELLOW}[-]          Author: CarlosAllberto          [-]{Fore.RESET}"))
+    # print(align(f"{Fore.YELLOW}[-]   GitHub: www.github.com/CarlosAllberto  [-]{Fore.RESET}"))
+    # print(align(f"[*]            *****************             [*]"))
+    # print(align(f"Projeto criado com o a intuito de ajudar\n iniciantes e profissionais a subir projetos \nno GitHub de forma super rápida.\n"))
   
 if __name__ == "__main__":
     banner()
```

### Comparing `git_assistente-0.1.8/git_assistente.egg-info/PKG-INFO` & `git_assistente-0.1.9/git_assistente.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-assistente
-Version: 0.1.8
+Version: 0.1.9
 Summary: Um assistente do Git para subir projetos no GitHub
 Home-page: UNKNOWN
 Author: CarlosAllberto
 Author-email: dasilvacarlosalberto344@gmail.com
 License: MIT License
 Keywords: git assistente
 Platform: UNKNOWN
```

### Comparing `git_assistente-0.1.8/git_assistente.egg-info/SOURCES.txt` & `git_assistente-0.1.9/git_assistente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git_assistente-0.1.8/setup.py` & `git_assistente-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='git_assistente',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT License',
     author='CarlosAllberto',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='dasilvacarlosalberto344@gmail.com',
     keywords='git assistente',
     description='Um assistente do Git para subir projetos no GitHub',
```

