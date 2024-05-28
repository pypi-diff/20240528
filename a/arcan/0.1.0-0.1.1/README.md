# Comparing `tmp/arcan-0.1.0.tar.gz` & `tmp/arcan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-0.1.0.tar", max compression
+gzip compressed data, was "arcan-0.1.1.tar", max compression
```

## Comparing `arcan-0.1.0.tar` & `arcan-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    11357 2024-05-13 04:54:28.035536 arcan-0.1.0/LICENSE
--rw-r--r--   0        0        0     4467 2024-05-13 04:54:28.035536 arcan-0.1.0/README.md
--rw-r--r--   0        0        0     2259 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/__init__.py
--rw-r--r--   0        0        0    10021 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/agents/__init__.py
--rw-r--r--   0        0        0     4216 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/agents/helpers.py
--rw-r--r--   0        0        0     3099 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/chains/__init__.py
--rw-r--r--   0        0        0     3141 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/llm/__init__.py
--rw-r--r--   0        0        0     2537 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/parser/__init__.py
--rw-r--r--   0        0        0     8775 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/prompts/__init__.py
--rw-r--r--   0        0        0     2996 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/router/__init__.py
--rw-r--r--   0        0        0    11488 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/router/routes.py
--rw-r--r--   0        0        0     1808 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/runnables/__init__.py
--rw-r--r--   0        0        0     1316 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/templates/__init__.py
--rw-r--r--   0        0        0     2724 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/tools/__init__.py
--rw-r--r--   0        0        0     5383 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/__init__.py
--rw-r--r--   0        0        0     1020 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/__init__.py
--rw-r--r--   0        0        0      626 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/chat_history.py
--rw-r--r--   0        0        0      794 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/conversation.py
--rw-r--r--   0        0        0     5777 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/user.py
--rw-r--r--   0        0        0     5707 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/session/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/session/auth.py
--rw-r--r--   0        0        0        0 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/__init__.py
--rw-r--r--   0        0        0     7390 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/scrapping.py
--rw-r--r--   0        0        0      411 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/search.py
--rw-r--r--   0        0        0     9082 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/vector_search.py
--rw-r--r--   0        0        0     1618 2024-05-13 04:54:28.039536 arcan-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6629 1970-01-01 00:00:00.000000 arcan-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 02:05:36.980345 arcan-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4467 2024-05-28 02:05:36.980345 arcan-0.1.1/README.md
+-rw-r--r--   0        0        0     2259 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/__init__.py
+-rw-r--r--   0        0        0    33800 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/agents/__init__.py
+-rw-r--r--   0        0        0     4216 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/agents/helpers.py
+-rw-r--r--   0        0        0     5587 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/agents/session.py
+-rw-r--r--   0        0        0     3099 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/chains/__init__.py
+-rw-r--r--   0        0        0     3332 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/llm/__init__.py
+-rw-r--r--   0        0        0     2537 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/parser/__init__.py
+-rw-r--r--   0        0        0     8775 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/prompts/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/router/__init__.py
+-rw-r--r--   0        0        0    11488 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/router/routes.py
+-rw-r--r--   0        0        0     1621 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/runnables/__init__.py
+-rw-r--r--   0        0        0     1316 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/templates/__init__.py
+-rw-r--r--   0        0        0     2724 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/ai/tools/__init__.py
+-rw-r--r--   0        0        0    12485 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/api/__init__.py
+-rw-r--r--   0        0        0     1408 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/api/auth.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/datamodel/__init__.py
+-rw-r--r--   0        0        0      629 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/datamodel/chat_history.py
+-rw-r--r--   0        0        0      797 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/datamodel/conversation.py
+-rw-r--r--   0        0        0     2109 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/datamodel/engine.py
+-rw-r--r--   0        0        0     5782 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/datamodel/user.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/spells/__init__.py
+-rw-r--r--   0        0        0     7390 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/spells/scrapping.py
+-rw-r--r--   0        0        0      411 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/spells/search.py
+-rw-r--r--   0        0        0     9082 2024-05-28 02:05:36.980345 arcan-0.1.1/arcan/spells/vector_search.py
+-rw-r--r--   0        0        0     1578 2024-05-28 02:05:36.984345 arcan-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6639 1970-01-01 00:00:00.000000 arcan-0.1.1/PKG-INFO
```

### Comparing `arcan-0.1.0/LICENSE` & `arcan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/README.md` & `arcan-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/__init__.py` & `arcan-0.1.1/arcan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typer import Typer, echo
 
 cli = Typer()
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 def get_arcan_version():
     try:
         import arcan
 
         return arcan.__version__
```

### Comparing `arcan-0.1.0/arcan/ai/agents/helpers.py` & `arcan-0.1.1/arcan/ai/agents/helpers.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/ai/chains/__init__.py` & `arcan-0.1.1/arcan/ai/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/ai/llm/__init__.py` & `arcan-0.1.1/arcan/ai/llm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # %%
 
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
+from langchain_community.chat_models import ChatOllama
 from langchain_groq import ChatGroq
 from langchain_openai import ChatOpenAI, OpenAI
 from pydantic import BaseModel
 
 
 class LLM(BaseModel):
     """Represents a Language Learning Model (LLM) configuration and its interaction logic.
@@ -65,14 +66,17 @@
         "ChatGroq": lambda **kwargs: ChatGroq(
             temperature=kwargs.get("temperature", 0.7),
             model_name=kwargs.get(
                 "model",
                 os.getenv("TOGETHER_MODEL_NAME", "llama3-8b-8192"),
             ),
         ),
+        "ChatOllama": lambda **kwargs: ChatOllama(
+            model=kwargs.get("model", os.getenv("OLLAMA_MODEL", "phi3")),
+        ),
     }
 
     @staticmethod
     def create_llm(provider: str, **kwargs: Any) -> Union[ChatOpenAI, OpenAI]:
         """Creates an LLM instance based on the specified provider.
 
         Args:
```

### Comparing `arcan-0.1.0/arcan/ai/parser/__init__.py` & `arcan-0.1.1/arcan/ai/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/ai/prompts/__init__.py` & `arcan-0.1.1/arcan/ai/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/ai/router/__init__.py` & `arcan-0.1.1/arcan/ai/router/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,19 +59,20 @@
         route = rl(query)
         strategy = self.response_strategies.get(route.name)
         if strategy:
             print(
                 f"Matched route: {route.name}, using strategy: {strategy.__class__.__name__}"
             )
             route_text = strategy.execute(query=query, user_id=user_id)
-            query += f" (SYSTEM NOTE: {route_text})"
-            return query
+            route_template = f" (SYSTEM NOTE: {route_text})"
+            query += route_template
+            return route_text, query
         else:
             print(f"No route found for query: {query}")
-        return query
+        return "No Router Matched", query
 
 
 # Initialize RouteManager with an encoder
 encoder = OpenAIEncoder()
 route_manager = RouteManager(encoder)
 
 # Dynamically adding routes to the RouteManager using the configuration (from routes.py)
@@ -85,9 +86,9 @@
 
     Args:
         query (str): The query to be processed.
 
     Returns:
         str: The response generated by the route manager.
     """
-    response = route_manager.get_response(query=query, user_id=user_id)
-    return response
+    response, route_text = route_manager.get_response(query=query, user_id=user_id)
+    return response, route_text
```

### Comparing `arcan-0.1.0/arcan/ai/router/routes.py` & `arcan-0.1.1/arcan/ai/router/routes.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/ai/templates/__init__.py` & `arcan-0.1.1/arcan/ai/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/ai/tools/__init__.py` & `arcan-0.1.1/arcan/ai/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/api/__init__.py` & `arcan-0.1.1/arcan/datamodel/user.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,207 +1,193 @@
 # %%
+import os
 from datetime import datetime, timedelta, timezone
-from typing import Annotated, Any, Dict, List, Optional, Union
+from typing import Annotated
 
-from dotenv import load_dotenv
-from fastapi import Depends, FastAPI, Form, HTTPException, Request, status
-from fastapi.middleware.cors import CORSMiddleware
-from fastapi.responses import RedirectResponse
-
-# %%
-from fastapi.security import (
-    HTTPAuthorizationCredentials,
-    HTTPBearer,
-    OAuth2PasswordBearer,
-    OAuth2PasswordRequestForm,
-)
-from langchain_core.messages import AIMessage, FunctionMessage, HumanMessage
-from langserve import add_routes
-from langserve.pydantic_v1 import BaseModel, Field
+from fastapi import Depends, FastAPI, HTTPException, status
+from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
+from jose import JWTError, jwt
+from passlib.context import CryptContext
 from pydantic import BaseModel
-from sqlalchemy.dialects.postgresql import insert
-from sqlalchemy.orm import Session
-from typing_extensions import Annotated
-
-from arcan.ai.agents import ArcanSpellsAgent
-from arcan.ai.llm import LLM
-from arcan.api.datamodel import get_db, get_db_context
-from arcan.api.datamodel.chat_history import ChatHistory
-from arcan.api.datamodel.conversation import Conversation
-from arcan.api.datamodel.user import (
-    ACCESS_TOKEN_EXPIRE_MINUTES,
-    TokenModel,
-    User,
-    UserInDB,
-    UserModel,
-    UserRepository,
-    UserService,
-    oauth2_scheme,
-    pwd_context,
-)
-from arcan.api.session import ArcanSession, run_agent
-
-# from arcan.api.session.auth import requires_auth
-from arcan.spells.vector_search import (
-    get_per_user_retriever,
-    per_req_config_modifier,
-    pgVectorStore,
-)
-
-auth_scheme = HTTPBearer()
-
-load_dotenv()
-
-
-app = FastAPI()
-
-
-# Set all CORS enabled origins
-app.add_middleware(
-    CORSMiddleware,
-    allow_origins=["*"],
-    allow_credentials=True,
-    allow_methods=["*"],
-    allow_headers=["*"],
-    expose_headers=["*"],
-)
-
-
-@app.get("/")
-async def redirect_root_to_docs():
-    return RedirectResponse("/docs")
-
-
-@app.get("/api/check")
-async def index():
-    return {"message": "Arcan is Running!"}
+from sqlalchemy import Boolean, Column, DateTime, ForeignKey, Integer, String, Text
+from sqlalchemy.orm import Session, relationship
 
+from arcan.datamodel.engine import Base, engine
 
-# %%
+pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")
 
+oauth2_scheme = OAuth2PasswordBearer(tokenUrl="token")
+
+# %%
+Base.metadata.create_all(engine)
+# %%
 
-class Input(BaseModel):
-    input: str
-    chat_history: List[Union[HumanMessage, AIMessage, FunctionMessage]] = Field(
-        ...,
-        extra={"widget": {"type": "chat", "input": "input", "output": "output"}},
+# to get a string like this run:
+# openssl rand -hex 32
+SECRET_KEY = os.environ.get("ARCANAI_API_KEY")
+ALGORITHM = "HS256"
+ACCESS_TOKEN_EXPIRE_MINUTES = 30
+
+
+class User(Base):
+    __tablename__ = "user"
+    __table_args__ = {"extend_existing": True}
+    username = Column(String, primary_key=True, index=True)
+    email = Column(String, nullable=True)
+    full_name = Column(String)
+    status = Column(String)
+    disabled = Column(Boolean)
+    created_at = Column(DateTime, default=datetime.utcnow)
+    hashed_password = Column(String)
+
+
+class Token(Base):
+    __tablename__ = "token"
+    __table_args__ = {"extend_existing": True}
+    id = Column(
+        Integer,
+        primary_key=True,
+        index=True,
     )
+    access_token = Column(String)
+    token_type = Column(String)
+    user_id = Column(String, ForeignKey("user.username"))
+    user = relationship("User", back_populates="tokens")
 
 
-class Output(BaseModel):
-    output: Any
+User.tokens = relationship("Token", order_by=Token.id, back_populates="user")
+# %%
 
 
-add_routes(
-    app=app,
-    runnable=ArcanSpellsAgent(
-        # database=SQLDatabase.from_uri(os.environ.get("SQLALCHEMY_URL"))
-    )
-    .agent_executor.with_types(input_type=Input, output_type=Output)
-    .with_config({"run_name": "agent"}),
-    path="/spells_agent",
-    enable_feedback_endpoint=True,
-)
-
-add_routes(
-    app,
-    LLM(provider="ChatOpenAI").llm,
-    per_req_config_modifier=per_req_config_modifier,
-    path="/openai",
-)
-
-add_routes(
-    app,
-    LLM(provider="ChatGroq").llm,
-    per_req_config_modifier=per_req_config_modifier,
-    path="/groq",
-)
-
-add_routes(
-    app,
-    LLM(provider="ChatTogetherAI").llm,
-    path="/together",
-)
-
-
-@app.post("/token")
-async def login_for_access_token(
-    form_data: Annotated[OAuth2PasswordRequestForm, Depends()],
-    session: Session = Depends(get_db),
-) -> TokenModel:
-    user_repo = UserRepository(session)
-    user_interface = UserService(user_repository=user_repo, pwd_context=pwd_context)
-    user = user_interface.authenticate_user(form_data.username, form_data.password)
-    if not user:
-        raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Incorrect username or password",
-            headers={"WWW-Authenticate": "Bearer"},
+class UserModel(BaseModel):
+    username: str
+    email: str | None = None
+    full_name: str | None = None
+    status: str | None = None
+    disabled: bool | None = None
+    created_at: datetime | None = None
+    hashed_password: str
+
+
+class TokenModel(BaseModel):
+    id: int
+    access_token: str
+    token_type: str
+    user_id: str
+    user: UserModel
+
+
+class TokenData(BaseModel):
+    username: str | None = None
+
+
+class UserInDB(BaseModel):
+    hashed_password: str
+
+
+class UserRepository:
+    def __init__(self, session: Session):
+        self.session = session
+
+    def add_user(self, user: User):
+        with self.session as db_session:
+            db_session.add(user)
+            db_session.commit()
+
+    def get_user(self, username: str):
+        with self.session as db_session:
+            return db_session.query(User).filter_by(username=username).first()
+
+    def update_user(self, user: User):
+        with self.session as db_session:
+            db_session.commit()
+
+    def delete_user(self, username: str):
+        with self.session as db_session:
+            user = self.get_user(username)
+            if user:
+                db_session.delete(user)
+                db_session.commit()
+
+
+class UserService:
+    def __init__(self, user_repository: UserRepository, pwd_context: CryptContext):
+        self.user_repository = user_repository
+        self.pwd_context = pwd_context
+
+    def authenticate_user(self, username, password):
+        user = self.user_repository.get_user(username)
+        if not user:
+            return False
+        if not self.verify_password(password, user.hashed_password):
+            return False
+        return user
+
+    def register_user(self, username, email, full_name, password):
+        user = User(
+            username=username,
+            email=email,
+            full_name=full_name,
+            disabled=False,
+            hashed_password=self.hash_password(password),
         )
-    access_token_expires = timedelta(minutes=ACCESS_TOKEN_EXPIRE_MINUTES)
-    access_token = user_interface.create_access_token(
-        data={"sub": user.username}, expires_delta=access_token_expires
-    )
-    return TokenModel(
-        id=1,
-        access_token=access_token,
-        token_type="bearer",
-        user_id=user.username,
-        user=user,
-    )
+        self.user_repository.add_user(user)
+
+    def hash_password(self, password):
+        return self.pwd_context.hash(password)
 
+    def verify_password(self, plain_password, hashed_password):
+        return self.pwd_context.verify(plain_password, hashed_password)
 
-async def get_current_active_user_from_request(
-    request: Request, session: Session = Depends(get_db)
-) -> UserModel:
-    """Get the current active user from the request."""
-    user_repo = UserRepository(session)
-    user_interface = UserService(user_repository=user_repo, pwd_context=pwd_context)
-    token = await oauth2_scheme(request)
-    user = user_interface.get_current_user(token=token)
-    if not user:
-        raise HTTPException(
+    def disable_user(self, username):
+        user = self.user_repository.get_user(username)
+        if user:
+            user.disabled = True
+            self.user_repository.update_user(user)
+
+    def enable_user(self, username):
+        user = self.user_repository.get_user(username)
+        if user:
+            user.disabled = False
+            self.user_repository.update_user(user)
+
+    def create_access_token(self, data: dict, expires_delta: timedelta | None = None):
+        to_encode = data.copy()
+        if expires_delta:
+            expire = datetime.now(timezone.utc) + expires_delta
+        else:
+            expire = datetime.now(timezone.utc) + timedelta(minutes=15)
+        to_encode.update({"exp": expire})
+        encoded_jwt = jwt.encode(to_encode, SECRET_KEY, algorithm=ALGORITHM)
+        return encoded_jwt
+
+    async def get_current_user(
+        self, token: Annotated[str, Depends(oauth2_scheme)]
+    ) -> str:
+        credentials_exception = HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Invalid authentication credentials",
+            detail="Could not validate credentials",
             headers={"WWW-Authenticate": "Bearer"},
         )
-    if user.disabled:
-        raise HTTPException(status_code=400, detail="Inactive user")
-    return user
-
-
-@app.get("/users/me/", response_model=UserModel)
-async def read_users_me(
-    current_user: Annotated[UserModel, Depends(get_current_active_user_from_request)],
-):
-    return current_user
-
-
-add_routes(
-    app,
-    get_per_user_retriever(vectorstore=pgVectorStore().get_vector_store()),
-    per_req_config_modifier=per_req_config_modifier,
-    enabled_endpoints=["invoke"],
-)
-
-# %%
-
-
-# @requires_auth
-@app.get("/api/chat")
-async def chat(
-    user_id: str,
-    query: str,
-    current_user: Annotated[UserModel, Depends(get_current_active_user_from_request)],
-    db: Session = Depends(get_db),
-):
-    arcan_session = ArcanSession(db)
-    response = run_agent(session=arcan_session, user_id=current_user, query=query)
-    return {"response": response}
-
-
-if __name__ == "__main__":
-    import uvicorn
+        try:
+            payload = jwt.decode(token, SECRET_KEY, algorithms=[ALGORITHM])
+            username: str = payload.get("sub")
+            if username is None:
+                raise credentials_exception
+            token_data = TokenData(username=username)
+        except JWTError:
+            raise credentials_exception
+        user = self.user_repository.get_user(username)
+        if user is None:
+            raise credentials_exception
+        return user
+
+    async def get_current_active_user(
+        self,
+        current_user: Annotated[User, Depends(get_current_user)],
+    ):
+        if current_user.disabled:
+            raise HTTPException(status_code=400, detail="Inactive user")
+        return current_user
 
-    uvicorn.run(app, host="localhost", port=8000)
 
 # %%
```

### Comparing `arcan-0.1.0/arcan/api/datamodel/chat_history.py` & `arcan-0.1.1/arcan/datamodel/chat_history.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 from sqlalchemy import Column, DateTime, String, Text
 
-from arcan.api.datamodel import Base, engine
+from arcan.datamodel.engine import Base, engine
 
 Base.metadata.create_all(engine)
 
 
 class ChatHistory(Base):
     """
     Represents the chat history for a sender.
```

### Comparing `arcan-0.1.0/arcan/api/datamodel/conversation.py` & `arcan-0.1.1/arcan/datamodel/conversation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 from sqlalchemy import Column, DateTime, Integer, String
 
-from arcan.api.datamodel import Base, engine
+from arcan.datamodel.engine import Base, engine
 
 Base.metadata.create_all(engine)
 
 
 class Conversation(Base):
     """
     Represents a conversation entity.
```

### Comparing `arcan-0.1.0/arcan/api/session/__init__.py` & `arcan-0.1.1/arcan/ai/agents/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,151 +1,154 @@
+# %%
+
 import ast
 import os
 import pickle
 import weakref
 from datetime import datetime
-from typing import Dict
+from typing import Any, Dict
 
-from fastapi import Depends
-from langchain.sql_database import SQLDatabase
 from sqlalchemy.dialects.postgresql import insert
-from sqlalchemy.exc import SQLAlchemyError
-from sqlalchemy.orm import Session
+from sqlalchemy.orm import Session, joinedload
 
-from arcan.ai.agents import ArcanAgent, ArcanSpellsAgent
-from arcan.api.datamodel.chat_history import ChatHistory
-from arcan.api.datamodel.conversation import Conversation
+from arcan.datamodel.chat_history import ChatHistory
+from arcan.datamodel.conversation import Conversation
+from arcan.datamodel.engine import SessionLocal
 
 
 class ArcanSession:
-    def __init__(self, database: Session):
-        """
-        Initializes a new instance of the ArcanSession class.
-
-        :param database: A callable that returns a new SQLAlchemy Session instance when called.
-        """
+    def __init__(self, database: callable = SessionLocal):
         self.database = database
         self.database_uri = os.environ.get("SQLALCHEMY_URL")
         self.agents: Dict[str, weakref.ref] = weakref.WeakValueDictionary()
 
-    def get_or_create_agent(
-        self, user_id: str, provided_agent: ArcanAgent = None
-    ) -> ArcanAgent:
-        """
-        Retrieves or creates a ArcanAgent for a given user_id.
-
-        :param user_id: The unique identifier for the user.
-        :return: An instance of ArcanAgent.
-        """
-        if provided_agent is None:
-            agent = self.agents.get(user_id)
-            chat_history = []
-
-            # Obtain a new database session
-            try:
-                chat_history = self.get_chat_history(user_id)
-            except Exception as e:
-                print(f"Error getting chat history for {user_id}: {e}")
-
-            if agent is not None and chat_history:
-                print(f"Using existing agent {agent}")
-            elif agent is None and chat_history:
-                print(f"Using reloaded agent with history {chat_history}")
-                agent = ArcanSpellsAgent(
-                    context=chat_history,
-                    user_id=user_id,
-                    # database=SQLDatabase.from_uri(self.database_uri)
-                )  # Initialize with chat history
-            elif agent is None and not chat_history:
-                print("Using a new agent")
-                agent = ArcanSpellsAgent(
-                    user_id=user_id,
-                )
-                #   database=SQLDatabase.from_uri(self.database_uri))  # Initialize without chat history
-
-            self.agents[user_id] = agent
-            return agent
-
-        else:
-            provided_agent.user_id = user_id
-            self.agents[user_id] = provided_agent
-            return provided_agent
+    def _get_session(self) -> Session:
+        if self.database is None:
+            raise ValueError("Database factory is not initialized.")
+        return self.database()
 
     def store_message(self, user_id: str, body: str, response: str):
-        """
-        Stores a message in the database.
-
-        :param user_id: The unique identifier for the user.
-        :param Body: The body of the message sent by the user.
-        :param response: The response generated by the system.
-        """
-        with self.database as db_session:
+        with self._get_session() as db_session:
             conversation = Conversation(sender=user_id, message=body, response=response)
             db_session.add(conversation)
             db_session.commit()
             print(f"Conversation #{conversation.id} stored in database")
 
     def store_chat_history(self, user_id, agent_history):
-        """
-        Stores or updates the chat history for a user in the database.
-
-        :param user_id: The unique identifier for the user.
-        :param agent_history: The chat history to be stored.
-        """
         history = pickle.dumps(agent_history)
-        # Upsert statement
         stmt = (
             insert(ChatHistory)
             .values(
                 sender=user_id,
                 history=str(history),
-                updated_at=datetime.utcnow(),  # Explicitly set updated_at on insert
+                updated_at=datetime.utcnow(),
             )
             .on_conflict_do_update(
-                index_elements=["sender"],  # Specify the conflict target
+                index_elements=["sender"],
                 set_={
-                    "history": str(history),  # Update the history field upon conflict
-                    "updated_at": datetime.utcnow(),  # Update the updated_at field upon conflict
+                    "history": str(history),
+                    "updated_at": datetime.utcnow(),
                 },
             )
         )
-        # Execute the upsert
-        with self.database as db:
+        with self._get_session() as db:
             db.execute(stmt)
             db.commit()
             print(f"Upsert chat history for user {user_id} with statement {stmt}")
 
     def get_chat_history(self, user_id: str) -> list:
-        """
-        Retrieves the chat history for a user from the database.
-
-        :param db_session: The SQLAlchemy Session instance.
-        :param user_id: The unique identifier for the user.
-        :return: A list representing the chat history.
-        """
-        with self.database as db_session:
+        with self._get_session() as db_session:
             history = (
                 db_session.query(ChatHistory)
+                # .options(joinedload(ChatHistory.history))
                 .filter(ChatHistory.sender == user_id)
                 .order_by(ChatHistory.updated_at.asc())
                 .all()
             ) or []
         if not history:
             return []
         chat_history = history[0].history
         loaded = pickle.loads(ast.literal_eval(chat_history))
         return loaded
 
-
-def run_agent(session: ArcanSession, query: str, user_id: str) -> Dict[str, str]:
-    print(f"Sending the LangChain response to user: {user_id}")
-    agent = session.get_or_create_agent(user_id)
-    # Get the generated text from the LangChain agent
-    response = agent.get_response(user_content=query)
-    # Store the conversation in the database
-    try:
-        session.store_message(user_id=user_id, body=query, response=response)
-        session.store_chat_history(user_id=user_id, agent_history=agent.chat_history)
-    except SQLAlchemyError as e:
-        session.database.rollback()
-        print(f"Error storing conversation in database: {e}")
-    return response
+    def rollback(self):
+        with self._get_session() as db:
+            db.rollback()
+            print("Rollback transaction")
+
+
+# class ArcanSession:
+#     def __init__(self, database: Session = None):
+#         """
+#         Initializes a new instance of the ArcanSession class.
+
+#         :param database: A callable that returns a new SQLAlchemy Session instance when called.
+#         """
+#         self.database = database
+#         self.database_uri = os.environ.get("SQLALCHEMY_URL")
+#         self.agents: Dict[str, weakref.ref] = weakref.WeakValueDictionary()
+
+# def store_message(self, user_id: str, body: str, response: str):
+#     """
+#     Stores a message in the database.
+
+#     :param user_id: The unique identifier for the user.
+#     :param Body: The body of the message sent by the user.
+#     :param response: The response generated by the system.
+#     """
+#     with self.database as db_session:
+#         conversation = Conversation(sender=user_id, message=body, response=response)
+#         db_session.add(conversation)
+#         db_session.commit()
+#         print(f"Conversation #{conversation.id} stored in database")
+
+#     def store_chat_history(self, user_id, agent_history):
+#         """
+#         Stores or updates the chat history for a user in the database.
+
+#         :param user_id: The unique identifier for the user.
+#         :param agent_history: The chat history to be stored.
+#         """
+#         history = pickle.dumps(agent_history)
+#         # Upsert statement
+#         stmt = (
+#             insert(ChatHistory)
+#             .values(
+#                 sender=user_id,
+#                 history=str(history),
+#                 updated_at=datetime.utcnow(),  # Explicitly set updated_at on insert
+#             )
+#             .on_conflict_do_update(
+#                 index_elements=["sender"],  # Specify the conflict target
+#                 set_={
+#                     "history": str(history),  # Update the history field upon conflict
+#                     "updated_at": datetime.utcnow(),  # Update the updated_at field upon conflict
+#                 },
+#             )
+#         )
+#         # Execute the upsert
+#         with self.database as db:
+#             db.execute(stmt)
+#             db.commit()
+#             print(f"Upsert chat history for user {user_id} with statement {stmt}")
+
+#     def get_chat_history(self, user_id: str) -> list:
+#         """
+#         Retrieves the chat history for a user from the database.
+
+#         :param db_session: The SQLAlchemy Session instance.
+#         :param user_id: The unique identifier for the user.
+#         :return: A list representing the chat history.
+#         """
+#         with self.database as db_session:
+#             history = (
+#                 db_session.query(ChatHistory)
+#                 .filter(ChatHistory.sender == user_id)
+#                 .order_by(ChatHistory.updated_at.asc())
+#                 .all()
+#             ) or []
+#         if not history:
+#             return []
+#         chat_history = history[0].history
+#         loaded = pickle.loads(ast.literal_eval(chat_history))
+#         return loaded
+# %%
```

### Comparing `arcan-0.1.0/arcan/spells/scrapping.py` & `arcan-0.1.1/arcan/spells/scrapping.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/arcan/spells/vector_search.py` & `arcan-0.1.1/arcan/spells/vector_search.py`

 * *Files identical despite different names*

### Comparing `arcan-0.1.0/pyproject.toml` & `arcan-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "arcan"
-version = "0.1.0"
+version = "0.1.1"
 description = "An AI web3 tooling platform for the decentralized customization and enhancement of AI agents"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 urllib3 = ">=1.26.16,<3.0.0"
 fastapi = "^0.110.0"
 openai = "^1.14.0"
 langchain = "^0.1.16"
 langchain-openai = "^0.0.8"
 uvicorn = "^0.28.0"
-pydantic = "<2" #">=1.10.13,<3.0.0"
+pydantic = ">=1.10.13,<2"
 python-dotenv = "^1.0.1"
 typing-extensions = "^4.9.0"
 pandas = "^2.2.1"
 sqlalchemy = "^2.0.27"
 psycopg2-binary = "^2.9.9"
 bs4 = "^0.0.2"
 selenium = "^4.18.1"
@@ -33,15 +33,14 @@
 pyngrok = "^7.1.3"
 numexpr = "^2.9.0"
 langchainhub = "^0.1.15"
 langchain-experimental = "^0.0.54"
 langchain-community = "^0.0.32"
 # langchain-together = "^0.0.2.post1"
 # langchain-fireworks = "^0.1.1"
-# semantic-router = "^0.0.28"
 modal = "^0.61.54"
 typer = "^0.9.0"
 langserve = {extras = ["all"], version = ">=0.0.30"} #"^0.1.1"
 langchain-groq = "^0.1.3"
 firecrawl-py = "^0.0.8"
 passlib = {extras = ["bcrypt"], version = "^1.7.4"}
 python-jose = {extras = ["cryptography"], version = "^3.3.0"}
```

### Comparing `arcan-0.1.0/PKG-INFO` & `arcan-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 0.1.0
+Version: 0.1.1
 Summary: An AI web3 tooling platform for the decentralized customization and enhancement of AI agents
 License: Apache 2.0
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 Requires-Dist: langserve[all] (>=0.0.30)
 Requires-Dist: modal (>=0.61.54,<0.62.0)
 Requires-Dist: numexpr (>=2.9.0,<3.0.0)
 Requires-Dist: openai (>=1.14.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: passlib[bcrypt] (>=1.7.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
-Requires-Dist: pydantic (<2)
+Requires-Dist: pydantic (>=1.10.13,<2)
 Requires-Dist: pymupdf (>=1.23.25,<2.0.0)
 Requires-Dist: pyngrok (>=7.1.3,<8.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: selenium (>=4.18.1,<5.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arcan Version: 0.1.0 Summary: An AI web3 tooling
+Metadata-Version: 2.1 Name: arcan Version: 0.1.1 Summary: An AI web3 tooling
 platform for the decentralized customization and enhancement of AI agents
 License: Apache 2.0 Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.9,<3.13 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: bs4
@@ -13,37 +13,38 @@
 Requires-Dist: langchain-experimental (>=0.0.54,<0.0.55) Requires-Dist:
 langchain-groq (>=0.1.3,<0.2.0) Requires-Dist: langchain-openai
 (>=0.0.8,<0.0.9) Requires-Dist: langchainhub (>=0.1.15,<0.2.0) Requires-Dist:
 langserve[all] (>=0.0.30) Requires-Dist: modal (>=0.61.54,<0.62.0) Requires-
 Dist: numexpr (>=2.9.0,<3.0.0) Requires-Dist: openai (>=1.14.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0) Requires-Dist: passlib[bcrypt]
 (>=1.7.4,<2.0.0) Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) Requires-Dist:
-pydantic (<2) Requires-Dist: pymupdf (>=1.23.25,<2.0.0) Requires-Dist: pyngrok
-(>=7.1.3,<8.0.0) Requires-Dist: python-decouple (>=3.8,<4.0) Requires-Dist:
-python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-jose[cryptography]
-(>=3.3.0,<4.0.0) Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-
-Dist: selenium (>=4.18.1,<5.0.0) Requires-Dist: sendgrid (>=6.11.0,<7.0.0)
-Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0) Requires-Dist: supabase
-(>=2.4.5,<3.0.0) Requires-Dist: twilio (>=9.0.0,<10.0.0) Requires-Dist: typer
-(>=0.9.0,<0.10.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0) Requires-
-Dist: urllib3 (>=1.26.16,<3.0.0) Requires-Dist: uvicorn (>=0.28.0,<0.29.0)
-Requires-Dist: wikipedia (>=1.4.0,<2.0.0) Description-Content-Type: text/
-markdown # Arcan ### AI web3 tooling platform for decentralized customization
-and enhancement of AI agents Arcan is a web3 tooling platform designed to
-customize and enhance AI agents by leveraging blockchain technology. With
-Arcan, developers can securely tie AI personalization to user-owned blockchain
-profiles, ensuring privacy and control while delivering tailored AI
-interactions. Check out the live demo at [arcanai.tech](https://arcanai.tech/).
-## Features - **Blockchain-Backed AI Personalization**: Integrate AI agents
-with blockchain to create a personalized experience that respects user
-ownership. - **Web3 Tooling**: A suite of tools that enable seamless
-interaction between AI agents and blockchain assets. - **Privacy-Centric
-Design**: Ensuring user data is encrypted and owned by the user, accessible
-only through user permission. - **Developer-Friendly**: Straightforward APIs to
-enable developers to focus on building unique AI experiences.
+pydantic (>=1.10.13,<2) Requires-Dist: pymupdf (>=1.23.25,<2.0.0) Requires-
+Dist: pyngrok (>=7.1.3,<8.0.0) Requires-Dist: python-decouple (>=3.8,<4.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-jose
+[cryptography] (>=3.3.0,<4.0.0) Requires-Dist: python-multipart
+(>=0.0.9,<0.0.10) Requires-Dist: selenium (>=4.18.1,<5.0.0) Requires-Dist:
+sendgrid (>=6.11.0,<7.0.0) Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
+Requires-Dist: supabase (>=2.4.5,<3.0.0) Requires-Dist: twilio
+(>=9.0.0,<10.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: typing-
+extensions (>=4.9.0,<5.0.0) Requires-Dist: urllib3 (>=1.26.16,<3.0.0) Requires-
+Dist: uvicorn (>=0.28.0,<0.29.0) Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
+Description-Content-Type: text/markdown # Arcan ### AI web3 tooling platform
+for decentralized customization and enhancement of AI agents Arcan is a web3
+tooling platform designed to customize and enhance AI agents by leveraging
+blockchain technology. With Arcan, developers can securely tie AI
+personalization to user-owned blockchain profiles, ensuring privacy and control
+while delivering tailored AI interactions. Check out the live demo at
+[arcanai.tech](https://arcanai.tech/). ## Features - **Blockchain-Backed AI
+Personalization**: Integrate AI agents with blockchain to create a personalized
+experience that respects user ownership. - **Web3 Tooling**: A suite of tools
+that enable seamless interaction between AI agents and blockchain assets. -
+**Privacy-Centric Design**: Ensuring user data is encrypted and owned by the
+user, accessible only through user permission. - **Developer-Friendly**:
+Straightforward APIs to enable developers to focus on building unique AI
+experiences.
                             _[_p_u_b_l_i_c_/_a_r_c_a_n___l_o_g_o_._s_v_g_]
     Unleash AI potential with Arcan â your gateway to blockchain-powered,
  personalized AI experiences. Code smart, own smarter. Visit the live demo at
                                  _a_r_c_a_n_a_i_._t_e_c_h.
 
 ## Built With - [Python](https://www.python.org/) - Backend programming
 language - [Rust](https://www.rust-lang.org/) - Smart contract programming
```

