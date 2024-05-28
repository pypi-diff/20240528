# Comparing `tmp/atlassian_modules-0.4.tar.gz` & `tmp/atlassian_modules-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlassian_modules-0.4.tar", last modified: Tue Mar 26 10:45:07 2024, max compression
+gzip compressed data, was "atlassian_modules-0.4.1.tar", last modified: Tue May 28 04:46:17 2024, max compression
```

## Comparing `atlassian_modules-0.4.tar` & `atlassian_modules-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pavan.bhatt   (503) staff       (20)        0 2024-03-26 10:45:07.478702 atlassian_modules-0.4/
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)    40148 2024-03-26 10:45:07.471652 atlassian_modules-0.4/PKG-INFO
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)    39920 2024-03-26 10:44:04.000000 atlassian_modules-0.4/README.md
-drwxr-xr-x   0 pavan.bhatt   (503) staff       (20)        0 2024-03-26 10:45:07.439146 atlassian_modules-0.4/atlassian_modules/
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)       21 2024-01-04 15:21:57.000000 atlassian_modules-0.4/atlassian_modules/__init__.py
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)    43984 2024-03-22 14:56:31.000000 atlassian_modules-0.4/atlassian_modules/helper.py
-drwxr-xr-x   0 pavan.bhatt   (503) staff       (20)        0 2024-03-26 10:45:07.468871 atlassian_modules-0.4/atlassian_modules.egg-info/
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)    40148 2024-03-26 10:45:07.000000 atlassian_modules-0.4/atlassian_modules.egg-info/PKG-INFO
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)      280 2024-03-26 10:45:07.000000 atlassian_modules-0.4/atlassian_modules.egg-info/SOURCES.txt
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)        1 2024-03-26 10:45:07.000000 atlassian_modules-0.4/atlassian_modules.egg-info/dependency_links.txt
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)       24 2024-03-26 10:45:07.000000 atlassian_modules-0.4/atlassian_modules.egg-info/requires.txt
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)       18 2024-03-26 10:45:07.000000 atlassian_modules-0.4/atlassian_modules.egg-info/top_level.txt
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)       38 2024-03-26 10:45:07.478901 atlassian_modules-0.4/setup.cfg
--rw-r--r--   0 pavan.bhatt   (503) staff       (20)      492 2024-03-26 10:44:04.000000 atlassian_modules-0.4/setup.py
+drwxr-xr-x   0 pavan.bhatt   (503) staff       (20)        0 2024-05-28 04:46:17.854090 atlassian_modules-0.4.1/
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)    40974 2024-05-28 04:46:17.848194 atlassian_modules-0.4.1/PKG-INFO
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)    40684 2024-05-28 04:42:39.000000 atlassian_modules-0.4.1/README.md
+drwxr-xr-x   0 pavan.bhatt   (503) staff       (20)        0 2024-05-28 04:46:17.811813 atlassian_modules-0.4.1/atlassian_modules/
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)       21 2024-01-04 15:21:57.000000 atlassian_modules-0.4.1/atlassian_modules/__init__.py
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)    43984 2024-03-22 14:56:31.000000 atlassian_modules-0.4.1/atlassian_modules/helper.py
+drwxr-xr-x   0 pavan.bhatt   (503) staff       (20)        0 2024-05-28 04:46:17.845175 atlassian_modules-0.4.1/atlassian_modules.egg-info/
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)    40974 2024-05-28 04:46:17.000000 atlassian_modules-0.4.1/atlassian_modules.egg-info/PKG-INFO
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)      280 2024-05-28 04:46:17.000000 atlassian_modules-0.4.1/atlassian_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)        1 2024-05-28 04:46:17.000000 atlassian_modules-0.4.1/atlassian_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)       24 2024-05-28 04:46:17.000000 atlassian_modules-0.4.1/atlassian_modules.egg-info/requires.txt
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)       18 2024-05-28 04:46:17.000000 atlassian_modules-0.4.1/atlassian_modules.egg-info/top_level.txt
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)       38 2024-05-28 04:46:17.854288 atlassian_modules-0.4.1/setup.cfg
+-rw-r--r--   0 pavan.bhatt   (503) staff       (20)      500 2024-05-28 04:45:50.000000 atlassian_modules-0.4.1/setup.py
```

### Comparing `atlassian_modules-0.4/PKG-INFO` & `atlassian_modules-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 Metadata-Version: 2.1
 Name: atlassian_modules
-Version: 0.4
-Summary: Modules for interacting with Atlassian products.
+Version: 0.4.1
+Summary: Modules for interacting with Atlassian cloud products.
 Home-page: 
 Author: Pavan Bhatt
 Author-email: pavanhbhatt1@gmail.com
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
 
 The best way to interact with Atlassian Jira/Confluence API.
 
+> **Note:** _This module is useful for the Atlassian Cloud_ <br>
+> Your URL should look like this https://domain.atlassian.net
+
+
 # Prerequisites
 ```python
 from atlassian_modules import JiraHelper # for Jira
 from atlassian_modules import  WikiHelper # for Wiki
 ```
 
 # Getting Started
 
 ## Connectivity to Atlassian Jira
 
 To initialize a connection to Jira, instantiate the `JiraHelper` class with your Jira URL, email, and API token:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 ```
 ______________________________________________________________________________
 ______________________________________________________________________________
 # Atlassian Jira
 ______________________________________________________________________________
 ______________________________________________________________________________
 ## 1. Create a Jira Ticket
 
 - You can create a new Jira ticket using the `create_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_url = jira_helper.create_ticket("PRJ", "Issue Summary", "Detailed issue description.", "Bug")
 if ticket_url:
     print(f"Ticket created: {ticket_url}")
 else:
     print("Failed to create ticket.")
 ```
@@ -56,15 +62,15 @@
 - `URL of the created ticket (str)`: If the ticket creation is successful, the function returns the URL to access the newly created ticket directly. 
 - `False`: If the ticket creation fails (for example, due to incorrect input parameters or server errors), the function returns `False`.
 ______________________________________________________________________________
 ## 2. Create a custom Jira Ticket
 - You can create a new custom Jira ticket using the `create_custom_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 # Define additional fields if necessary
 additional_fields = {
     "customfield_12345": "Custom value",
     "labels": ["label1", "label2"]
 }
 
@@ -88,15 +94,15 @@
 Return:
 - `URL of the created ticket` (str): If the ticket creation is successful, the function returns the URL to access the newly created ticket directly. This allows for immediate navigation to the ticket for review or further action.
 - `False`: If the ticket creation process fails, whether due to incorrect input parameters, server errors, or issues with the additional fields, the function returns `False`. This indicates that the ticket was not created and provides an opportunity to address any issues before retrying.
 ______________________________________________________________________________
 ## 3. Update the Jira ticket with inbuilt and custom fields
 - You can update any custom field of Jira ticket using the `update_ticket_with_fields` method:
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 # Define the additional fields you want to update
 additional_fields = {
     "customfield_12345": "New custom value",
     "labels": ["newlabel1", "newlabel2"]
 }
 
@@ -118,15 +124,15 @@
 - `False` otherwise. If the ticket update fails (for example, due to incorrect ticket ID, fields that cannot be updated, or server errors), the function returns `False`, and additional error information is printed to help diagnose the issue.
 ______________________________________________________________________________
 ## 3. Delete a Jira Ticket
 
 - To delete a ticket, use the `delete_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 if jira_helper.delete_ticket(ticket_key):
     print("Ticket deleted successfully.")
 else:
     print("Failed to delete ticket or ticket does not exist.")
 ```
@@ -139,15 +145,15 @@
 Return:
 - `True`: If the ticket is successfully deleted. This is indicated by a `204` HTTP status code from the JIRA API, meaning "`No Content`" but signifying successful deletion. 
 - `False`: If the deletion fails, which can occur if the ticket does not exist or if there's an issue with the API request (e.g., permissions, invalid ticket key). This is communicated by returning `False`.
 ______________________________________________________________________________
 ## 4. Get Transition ID
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 transition_name = "Close"
 transition_id = jira_helper.get_transitions(ticket_key, transition_name)
 if transition_id:
     print(f"Transition ID for '{transition_name}' is {transition_id}.")
 else:
@@ -166,15 +172,15 @@
 - `False`: If the specified transition is not found for the ticket, or if there is any failure in fetching transitions (e.g., due to an invalid ticket key, network issues, or server errors), the function returns `False`.
 ______________________________________________________________________________
 ## 5. Transition a Jira Ticket
 
 - To transition a ticket to a different status, use the `transition_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 transition_input = "Done"  # Can be a transition name like 'Done' or an ID like '31'
 if jira_helper.transition_ticket(ticket_key, transition_input):
     print("Ticket transitioned successfully.")
 else:
     print("Failed to transition ticket.")
@@ -193,15 +199,15 @@
 
 ______________________________________________________________________________
 ## 6. If exist a Jira Ticket
 
 - To check if a ticket exist, use the `if_ticket_exist` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 if jira_helper.if_ticket_exist(ticket_key):
     print("The ticket exists.")
 else:
     print("The ticket does not exist.")
 ```
@@ -216,15 +222,15 @@
 - `False`: If the ticket does not exist or if there was an error in checking. A `404` HTTP status code indicates the ticket does not exist. Other status codes indicate a failure in the request to check the ticket.
 ______________________________________________________________________________
 ## 7. Comment on a Jira ticket
 
 - To comment on the ticket, use the `comment_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 comment_text = "This is an example comment."
 comment_url = jira_helper.comment_ticket(ticket_key, comment_text)
 if comment_url:
     print(f"Comment added successfully: {comment_url}")
 else:
@@ -242,15 +248,15 @@
 - `False`: If adding the comment fails. This could be because the ticket does not exist, the comment text is invalid, or there was an error in the request itself. In such cases, the function returns `False`.
 ______________________________________________________________________________
 ## 8. Pass the JQL and get the ticket array
 
 - To query tickets using JQL, use the `jql_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 jql_query = "project = PRJ AND status = 'Open'"
 max_results = 100  # Optional
 ticket_keys = jira_helper.jql_ticket(jql_query, max_results)
 if ticket_keys:
     print(f"Found tickets: {', '.join(ticket_keys)}")
 else:
@@ -271,15 +277,15 @@
 ______________________________________________________________________________
 # Atlassian Wiki
 ______________________________________________________________________________
 ______________________________________________________________________________
 ## 1. Creating a wiki page
 - To create wiki page, use the `create_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(CONFLUENCE_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 space_key = "DEV"
 title = "API Documentation"
 content = "<p>This is the API documentation for our project.</p>"
 parent_page_id = 123456  # Optional
 page_url = wiki_helper.create_wiki_page(space_key, title, content, parent_page_id)
 if page_url:
@@ -299,15 +305,15 @@
 Return: 
 - `URL of the created Confluence page` (str): If the page creation is successful, the function returns the URL to access the newly created page. This is indicated by a `200` HTTP status code. 
 - `False`: If the page creation fails. This could be due to various issues, such as invalid input parameters, permissions problems, or server errors. In such cases, the function returns `False`.
 ______________________________________________________________________________
 ## 2. Duplicate a wiki page
 - To duplicate wiki page, use the `duplicate_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 source_page_id = "12345"  # Example source page ID
 target_space_key = "TGT"  # Example target space key
 target_title = "Duplicated Page Title"  # New title for the duplicated page
 target_parent_page_id = "67890"  # Optional parent page ID for the new page
 
 duplicated_page_url = wiki_helper.duplicate_wiki_page(source_page_id, target_space_key, target_title, target_parent_page_id)
@@ -327,15 +333,15 @@
 Return: 
 - `URL of the duplicated Confluence page` (str): If the duplication is successful, the method returns the URL to access the newly created duplicated page. This URL is constructed from the response of the page creation process. 
 - `None`: If the duplication fails at any point (e.g., retrieving content from the source page, creating the new page), the method returns `None`. This indicates that the operation was not successful, and no new page was created.
 ______________________________________________________________________________
 ## 3. Create a wiki page from template
 - To create a wiki page from template use the `create_page_from_template` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 template_id = "12345"  # Example template ID
 space_key = "TGT"  # Example space key
 title = "New Page from Template"  # Title for the new page
 parent_page_id = "67890"  # Optional parent page ID
 
 created_page_url = wiki_helper.create_page_from_template(template_id, space_key, title, parent_page_id)
@@ -354,15 +360,15 @@
 Return: 
 - `URL of the created Confluence page` (str): If the page creation is successful, the function returns the URL to access the newly created page. This indicates that the page was created successfully and is accessible at the returned URL. 
 - `None` or `False`: If the page creation fails, due to reasons such as template retrieval failure, duplicate title, or any error in the creation process, the function returns `None` or `False`. This indicates that no new page was created.
 ______________________________________________________________________________
 ## 4. Move wiki page from one location to another
 - To move wiki page from one location to another location without changing title use `move_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "12345"  # Example page ID to be moved
 target_space_key = "NEWSPACE"  # Target space key
 target_position = "append"  # Position of the page relative to the parent page ('append', 'above', 'below')
 target_parent_page_id = "67890"  # Optional new parent page ID
 
 moved_page_url = wiki_helper.move_wiki_page(page_id, target_space_key, target_position, target_parent_page_id)
@@ -381,15 +387,15 @@
 Return: 
 - `URL of the moved Confluence page` (str): If the move operation is successful, the function returns the URL to access the moved page. This indicates that the page was successfully moved to the new space and position. 
 - `None` or `False`: If the move operation fails, due to reasons such as an error retrieving the current page details, an error in the move operation, or inability to retrieve the moved page URL, the function returns `None` or `False`. This indicates that the page was not successfully moved.
 ______________________________________________________________________________
 ## 5. Check if wiki page exist
 - To move wiki page from one location to another location without changing title use `move_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 title = "Example Page Title"  # Title of the Confluence wiki page to check
 space_key = "EX"  # Key of the Confluence space
 
 if wiki_helper.wiki_page_exists(title, space_key):
     print(f"The page '{title}' exists in space '{space_key}'.")
 else:
@@ -403,15 +409,15 @@
 Return: 
 - `True`: If the page exists. This is determined by the presence of results matching the specified title in the specified space. 
 - `False`: If the page does not exist or if there was an error during the request. This could be due to the specified page not being found in the given space or an issue with the Confluence API response.
 ______________________________________________________________________________
 ## 6. Retrieve all child pages
 - Recursively retrieve all descendant pages of a given parent page ID.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 parent_id = "12345"  # Example parent page ID
 child_pages = wiki_helper.get_child_pages_recursive(parent_id)
 if child_pages:
     print("Child pages found:")
     for page in child_pages:
         print(f"Title: {page['title']}, ID: {page['id']}, Parent ID: {page['parentid']}")
@@ -428,15 +434,15 @@
 Return: 
 - `List of child pages`: Returns a list of dictionaries, each containing the title, ID, and parent ID of each descendant page found. This allows for a comprehensive view of the hierarchy and content under the specified parent page. 
 - If the retrieval fails at any point (due to an error in fetching child pages, for instance), the recursive fetching process is designed to continue for other branches of the tree, aiming to return as complete a list as possible of descendant pages.
 ______________________________________________________________________________
 ## 7. Get wiki page ID
 - Retrieve the ID of a Confluence wiki page by its title.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 title = "Example Page"  # Title of the Confluence wiki page to search for
 space_key = "EX"  # Key of the Confluence space
 
 page_id = wiki_helper.get_page_id(title, space_key)
 if page_id:
     print(f"Found page '{title}' with ID: {page_id} in space '{space_key}'.")
@@ -455,15 +461,15 @@
 Return:
 - `ID of the page` (str): If a page with the specified title is found in the given space, the function returns the ID of the page. 
 - `False`: If no page is found with the given title in the specified space, or if there was an error during the request, the function returns `False`.
 ______________________________________________________________________________
 ## 8. Replace word in wiki
 - Replace all occurrences of a string in a Confluence wiki page.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 from_string = "old text"  # Text to be replaced
 to_string = "new text"  # Replacement text
 
 if wiki_helper.replace_in_page(page_id, from_string, to_string):
     print(f"Replaced all occurrences of '{from_string}' with '{to_string}' in page ID: {page_id}.")
@@ -483,15 +489,15 @@
 Return:
 - `True`: If the replacement operation was successful, whether replacements were made or not (including the case where the `from_string` was not found). 
 - `False`: If there was a failure at any point during the process, such as an error fetching the page content, or updating the page with the new content.
 ______________________________________________________________________________
 ## 9. Fetch tables from wiki
 - Fetch all tables from a Confluence wiki page.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 tables_json = wiki_helper.get_tables_from_page(page_id)
 if tables_json:
     print("Found tables on the page:")
     print(tables_json)
@@ -506,15 +512,15 @@
 Return:
 - JSON structure: Returns a JSON string that represents all the tables found on the page. Each table is structured into a JSON object with keys representing the table headers and values representing the row data. If multiple tables are found, they are indexed as `table1`, `table2`, etc., in the JSON structure. 
 - If the fetching fails (due to an unsuccessful API call) or if no tables are found on the page, the function returns an empty JSON object (`{}`).
 ______________________________________________________________________________
 ## 10. Replace the whole wiki page
 - Replace the entire Confluence wiki page with the new content
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "12345"  # Example page ID
 new_content = "<p>This is the new content for the page.</p>"  # HTML content
 
 if wiki_helper.update_wiki_page(page_id, new_content):
     print(f"Page ID: {page_id} was updated successfully.")
 else:
@@ -529,15 +535,15 @@
 Return:
 - `True`: If the page content update is successful. This is indicated by a status code of `200` from the Confluence REST API, showing that the update request was processed correctly. 
 - `False`: If the update fails. This could be due to various reasons such as an invalid page ID, issues with the Confluence server, or improper formatting of the new content. Failure is indicated by any status code other than `200`, and the method prints the error details received from the server.
 ______________________________________________________________________________
 ## 11. Get parent page ID
 - Retrieve the parent ID of a Confluence wiki page by passed page ID.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 parent_id = wiki_helper.get_parent_page_id(page_id)
 if parent_id:
     print(f"Parent page ID for page ID {page_id}: {parent_id}")
 else:
@@ -552,15 +558,15 @@
 Return:
 - `ID of the parent page` (str): If the specified page has a parent page, the method returns the ID of the parent page. This is useful for understanding the hierarchy of pages within Confluence spaces. 
 - `False`: If no parent page exists for the specified page or if there was an error in the fetch operation (such as an invalid page ID or a problem with the Confluence server), the method returns False. This helps to identify pages that are at the top level of their space or when an issue occurs with the retrieval process.
 ______________________________________________________________________________
 ## 12. Add Table of Content (TOC) in wiki page
 - Add a Table of Contents (TOC) to a Confluence wiki page if it doesn't already have one.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 result_message = wiki_helper.add_toc_to_page(page_id)
 print(result_message)
 ```
 Parameter
@@ -569,15 +575,15 @@
 Output and Return
 - The function returns a **message** indicating the operation's result. This could be a confirmation that the TOC was added successfully, a message stating that the TOC already exists, or an error message if the operation failed. 
 - **Error Handling**: If there are issues fetching the page data or updating the page, the function provides detailed error messages including the status code and response text from Confluence's API. This is helpful for diagnosing problems with the operation.
 ______________________________________________________________________________
 ## 13. Add row to the existing table in wiki page (beta)
 - Pass the header to identify the table and then add the row to that identified table
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 page_id = "123456"  # Example page ID
 headers = ["Header1", "Header2", "Header3"]  # The headers of the table you're targeting
 row_data = ["Data1", "Data2", "Data3"]  # The data for the new row
 
 result_message = wiki_helper.add_row_to_table(page_id, headers, row_data)
 print(result_message)
 ```
@@ -589,15 +595,15 @@
 Output and Return
 - The function returns a message indicating the result of the operation. This could be a confirmation of successful row addition, or an error message detailing why the operation failed.
 
 ______________________________________________________________________________
 ## 14. Add/Update row to the existing table in wiki page (beta)
 - Pass the header to identify the table and then add/update the row to that identified table
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 headers = ["Cluster Name", "Component Name", "Next Version"]  # The headers of your table
 new_row_data = ["Cluster1", "ComponentA", "v2.0"]  # Data for the new or updated row
 
 result_message = wiki_helper.update_or_add_table_row(page_id, headers, new_row_data)
 print(result_message)
@@ -611,14 +617,22 @@
 ______________________________________________________________________________
 # Data Privacy Note
 
 🔒 **We respect your privacy**: This module does **not** store any of your data anywhere. It simply interacts with the Atlassian Jira API to perform the requested operations. Ensure you manage your connection details securely.
 
 # Release Notes
 
+## Latest Release: 0.4.1 (28 May 2024)
+- Revision in documentation for better understanding
+  - Based on the internal design now `JIRA_URL`, `CONFLUENCE_URL` is replaced with `ATLASSIAN_URL`
+  - Technically we are using `https://domain.atlassian.net` only to address Jira and Wiki both
+  - This is mentioned in the top of the document as well
+- Beta Features (Continued from previous release):
+  - Beta functions `wiki_helper.add_row_to_table` & `wiki_helper.update_or_add_table_row` for improved table management.
+
 ## Latest Release: 0.4 (21 Mar 2024)
 - New Features:
   - JIRA Integration Enhancements:
     - Custom Ticket Creation: The `create_custom_ticket` function has been introduced, allowing for more flexible ticket creation in JIRA projects. This function supports additional fields, enabling users to specify custom data during ticket creation. 
     - Ticket Field Updates: The `update_ticket_with_fields` method has been added, offering the ability to update existing tickets with new or modified fields. This feature is crucial for maintaining accurate and up-to-date ticket information.
 - Beta Features (Continued from previous release):
   - Beta functions `wiki_helper.add_row_to_table` & `wiki_helper.update_or_add_table_row` for improved table management.
```

### Comparing `atlassian_modules-0.4/README.md` & `atlassian_modules-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 The best way to interact with Atlassian Jira/Confluence API.
 
+> **Note:** _This module is useful for the Atlassian Cloud_ <br>
+> Your URL should look like this https://domain.atlassian.net
+
+
 # Prerequisites
 ```python
 from atlassian_modules import JiraHelper # for Jira
 from atlassian_modules import  WikiHelper # for Wiki
 ```
 
 # Getting Started
 
 ## Connectivity to Atlassian Jira
 
 To initialize a connection to Jira, instantiate the `JiraHelper` class with your Jira URL, email, and API token:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 ```
 ______________________________________________________________________________
 ______________________________________________________________________________
 # Atlassian Jira
 ______________________________________________________________________________
 ______________________________________________________________________________
 ## 1. Create a Jira Ticket
 
 - You can create a new Jira ticket using the `create_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_url = jira_helper.create_ticket("PRJ", "Issue Summary", "Detailed issue description.", "Bug")
 if ticket_url:
     print(f"Ticket created: {ticket_url}")
 else:
     print("Failed to create ticket.")
 ```
@@ -47,15 +51,15 @@
 - `URL of the created ticket (str)`: If the ticket creation is successful, the function returns the URL to access the newly created ticket directly. 
 - `False`: If the ticket creation fails (for example, due to incorrect input parameters or server errors), the function returns `False`.
 ______________________________________________________________________________
 ## 2. Create a custom Jira Ticket
 - You can create a new custom Jira ticket using the `create_custom_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 # Define additional fields if necessary
 additional_fields = {
     "customfield_12345": "Custom value",
     "labels": ["label1", "label2"]
 }
 
@@ -79,15 +83,15 @@
 Return:
 - `URL of the created ticket` (str): If the ticket creation is successful, the function returns the URL to access the newly created ticket directly. This allows for immediate navigation to the ticket for review or further action.
 - `False`: If the ticket creation process fails, whether due to incorrect input parameters, server errors, or issues with the additional fields, the function returns `False`. This indicates that the ticket was not created and provides an opportunity to address any issues before retrying.
 ______________________________________________________________________________
 ## 3. Update the Jira ticket with inbuilt and custom fields
 - You can update any custom field of Jira ticket using the `update_ticket_with_fields` method:
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 # Define the additional fields you want to update
 additional_fields = {
     "customfield_12345": "New custom value",
     "labels": ["newlabel1", "newlabel2"]
 }
 
@@ -109,15 +113,15 @@
 - `False` otherwise. If the ticket update fails (for example, due to incorrect ticket ID, fields that cannot be updated, or server errors), the function returns `False`, and additional error information is printed to help diagnose the issue.
 ______________________________________________________________________________
 ## 3. Delete a Jira Ticket
 
 - To delete a ticket, use the `delete_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 if jira_helper.delete_ticket(ticket_key):
     print("Ticket deleted successfully.")
 else:
     print("Failed to delete ticket or ticket does not exist.")
 ```
@@ -130,15 +134,15 @@
 Return:
 - `True`: If the ticket is successfully deleted. This is indicated by a `204` HTTP status code from the JIRA API, meaning "`No Content`" but signifying successful deletion. 
 - `False`: If the deletion fails, which can occur if the ticket does not exist or if there's an issue with the API request (e.g., permissions, invalid ticket key). This is communicated by returning `False`.
 ______________________________________________________________________________
 ## 4. Get Transition ID
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 transition_name = "Close"
 transition_id = jira_helper.get_transitions(ticket_key, transition_name)
 if transition_id:
     print(f"Transition ID for '{transition_name}' is {transition_id}.")
 else:
@@ -157,15 +161,15 @@
 - `False`: If the specified transition is not found for the ticket, or if there is any failure in fetching transitions (e.g., due to an invalid ticket key, network issues, or server errors), the function returns `False`.
 ______________________________________________________________________________
 ## 5. Transition a Jira Ticket
 
 - To transition a ticket to a different status, use the `transition_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 transition_input = "Done"  # Can be a transition name like 'Done' or an ID like '31'
 if jira_helper.transition_ticket(ticket_key, transition_input):
     print("Ticket transitioned successfully.")
 else:
     print("Failed to transition ticket.")
@@ -184,15 +188,15 @@
 
 ______________________________________________________________________________
 ## 6. If exist a Jira Ticket
 
 - To check if a ticket exist, use the `if_ticket_exist` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 if jira_helper.if_ticket_exist(ticket_key):
     print("The ticket exists.")
 else:
     print("The ticket does not exist.")
 ```
@@ -207,15 +211,15 @@
 - `False`: If the ticket does not exist or if there was an error in checking. A `404` HTTP status code indicates the ticket does not exist. Other status codes indicate a failure in the request to check the ticket.
 ______________________________________________________________________________
 ## 7. Comment on a Jira ticket
 
 - To comment on the ticket, use the `comment_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 comment_text = "This is an example comment."
 comment_url = jira_helper.comment_ticket(ticket_key, comment_text)
 if comment_url:
     print(f"Comment added successfully: {comment_url}")
 else:
@@ -233,15 +237,15 @@
 - `False`: If adding the comment fails. This could be because the ticket does not exist, the comment text is invalid, or there was an error in the request itself. In such cases, the function returns `False`.
 ______________________________________________________________________________
 ## 8. Pass the JQL and get the ticket array
 
 - To query tickets using JQL, use the `jql_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 jql_query = "project = PRJ AND status = 'Open'"
 max_results = 100  # Optional
 ticket_keys = jira_helper.jql_ticket(jql_query, max_results)
 if ticket_keys:
     print(f"Found tickets: {', '.join(ticket_keys)}")
 else:
@@ -262,15 +266,15 @@
 ______________________________________________________________________________
 # Atlassian Wiki
 ______________________________________________________________________________
 ______________________________________________________________________________
 ## 1. Creating a wiki page
 - To create wiki page, use the `create_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(CONFLUENCE_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 space_key = "DEV"
 title = "API Documentation"
 content = "<p>This is the API documentation for our project.</p>"
 parent_page_id = 123456  # Optional
 page_url = wiki_helper.create_wiki_page(space_key, title, content, parent_page_id)
 if page_url:
@@ -290,15 +294,15 @@
 Return: 
 - `URL of the created Confluence page` (str): If the page creation is successful, the function returns the URL to access the newly created page. This is indicated by a `200` HTTP status code. 
 - `False`: If the page creation fails. This could be due to various issues, such as invalid input parameters, permissions problems, or server errors. In such cases, the function returns `False`.
 ______________________________________________________________________________
 ## 2. Duplicate a wiki page
 - To duplicate wiki page, use the `duplicate_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 source_page_id = "12345"  # Example source page ID
 target_space_key = "TGT"  # Example target space key
 target_title = "Duplicated Page Title"  # New title for the duplicated page
 target_parent_page_id = "67890"  # Optional parent page ID for the new page
 
 duplicated_page_url = wiki_helper.duplicate_wiki_page(source_page_id, target_space_key, target_title, target_parent_page_id)
@@ -318,15 +322,15 @@
 Return: 
 - `URL of the duplicated Confluence page` (str): If the duplication is successful, the method returns the URL to access the newly created duplicated page. This URL is constructed from the response of the page creation process. 
 - `None`: If the duplication fails at any point (e.g., retrieving content from the source page, creating the new page), the method returns `None`. This indicates that the operation was not successful, and no new page was created.
 ______________________________________________________________________________
 ## 3. Create a wiki page from template
 - To create a wiki page from template use the `create_page_from_template` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 template_id = "12345"  # Example template ID
 space_key = "TGT"  # Example space key
 title = "New Page from Template"  # Title for the new page
 parent_page_id = "67890"  # Optional parent page ID
 
 created_page_url = wiki_helper.create_page_from_template(template_id, space_key, title, parent_page_id)
@@ -345,15 +349,15 @@
 Return: 
 - `URL of the created Confluence page` (str): If the page creation is successful, the function returns the URL to access the newly created page. This indicates that the page was created successfully and is accessible at the returned URL. 
 - `None` or `False`: If the page creation fails, due to reasons such as template retrieval failure, duplicate title, or any error in the creation process, the function returns `None` or `False`. This indicates that no new page was created.
 ______________________________________________________________________________
 ## 4. Move wiki page from one location to another
 - To move wiki page from one location to another location without changing title use `move_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "12345"  # Example page ID to be moved
 target_space_key = "NEWSPACE"  # Target space key
 target_position = "append"  # Position of the page relative to the parent page ('append', 'above', 'below')
 target_parent_page_id = "67890"  # Optional new parent page ID
 
 moved_page_url = wiki_helper.move_wiki_page(page_id, target_space_key, target_position, target_parent_page_id)
@@ -372,15 +376,15 @@
 Return: 
 - `URL of the moved Confluence page` (str): If the move operation is successful, the function returns the URL to access the moved page. This indicates that the page was successfully moved to the new space and position. 
 - `None` or `False`: If the move operation fails, due to reasons such as an error retrieving the current page details, an error in the move operation, or inability to retrieve the moved page URL, the function returns `None` or `False`. This indicates that the page was not successfully moved.
 ______________________________________________________________________________
 ## 5. Check if wiki page exist
 - To move wiki page from one location to another location without changing title use `move_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 title = "Example Page Title"  # Title of the Confluence wiki page to check
 space_key = "EX"  # Key of the Confluence space
 
 if wiki_helper.wiki_page_exists(title, space_key):
     print(f"The page '{title}' exists in space '{space_key}'.")
 else:
@@ -394,15 +398,15 @@
 Return: 
 - `True`: If the page exists. This is determined by the presence of results matching the specified title in the specified space. 
 - `False`: If the page does not exist or if there was an error during the request. This could be due to the specified page not being found in the given space or an issue with the Confluence API response.
 ______________________________________________________________________________
 ## 6. Retrieve all child pages
 - Recursively retrieve all descendant pages of a given parent page ID.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 parent_id = "12345"  # Example parent page ID
 child_pages = wiki_helper.get_child_pages_recursive(parent_id)
 if child_pages:
     print("Child pages found:")
     for page in child_pages:
         print(f"Title: {page['title']}, ID: {page['id']}, Parent ID: {page['parentid']}")
@@ -419,15 +423,15 @@
 Return: 
 - `List of child pages`: Returns a list of dictionaries, each containing the title, ID, and parent ID of each descendant page found. This allows for a comprehensive view of the hierarchy and content under the specified parent page. 
 - If the retrieval fails at any point (due to an error in fetching child pages, for instance), the recursive fetching process is designed to continue for other branches of the tree, aiming to return as complete a list as possible of descendant pages.
 ______________________________________________________________________________
 ## 7. Get wiki page ID
 - Retrieve the ID of a Confluence wiki page by its title.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 title = "Example Page"  # Title of the Confluence wiki page to search for
 space_key = "EX"  # Key of the Confluence space
 
 page_id = wiki_helper.get_page_id(title, space_key)
 if page_id:
     print(f"Found page '{title}' with ID: {page_id} in space '{space_key}'.")
@@ -446,15 +450,15 @@
 Return:
 - `ID of the page` (str): If a page with the specified title is found in the given space, the function returns the ID of the page. 
 - `False`: If no page is found with the given title in the specified space, or if there was an error during the request, the function returns `False`.
 ______________________________________________________________________________
 ## 8. Replace word in wiki
 - Replace all occurrences of a string in a Confluence wiki page.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 from_string = "old text"  # Text to be replaced
 to_string = "new text"  # Replacement text
 
 if wiki_helper.replace_in_page(page_id, from_string, to_string):
     print(f"Replaced all occurrences of '{from_string}' with '{to_string}' in page ID: {page_id}.")
@@ -474,15 +478,15 @@
 Return:
 - `True`: If the replacement operation was successful, whether replacements were made or not (including the case where the `from_string` was not found). 
 - `False`: If there was a failure at any point during the process, such as an error fetching the page content, or updating the page with the new content.
 ______________________________________________________________________________
 ## 9. Fetch tables from wiki
 - Fetch all tables from a Confluence wiki page.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 tables_json = wiki_helper.get_tables_from_page(page_id)
 if tables_json:
     print("Found tables on the page:")
     print(tables_json)
@@ -497,15 +501,15 @@
 Return:
 - JSON structure: Returns a JSON string that represents all the tables found on the page. Each table is structured into a JSON object with keys representing the table headers and values representing the row data. If multiple tables are found, they are indexed as `table1`, `table2`, etc., in the JSON structure. 
 - If the fetching fails (due to an unsuccessful API call) or if no tables are found on the page, the function returns an empty JSON object (`{}`).
 ______________________________________________________________________________
 ## 10. Replace the whole wiki page
 - Replace the entire Confluence wiki page with the new content
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "12345"  # Example page ID
 new_content = "<p>This is the new content for the page.</p>"  # HTML content
 
 if wiki_helper.update_wiki_page(page_id, new_content):
     print(f"Page ID: {page_id} was updated successfully.")
 else:
@@ -520,15 +524,15 @@
 Return:
 - `True`: If the page content update is successful. This is indicated by a status code of `200` from the Confluence REST API, showing that the update request was processed correctly. 
 - `False`: If the update fails. This could be due to various reasons such as an invalid page ID, issues with the Confluence server, or improper formatting of the new content. Failure is indicated by any status code other than `200`, and the method prints the error details received from the server.
 ______________________________________________________________________________
 ## 11. Get parent page ID
 - Retrieve the parent ID of a Confluence wiki page by passed page ID.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 parent_id = wiki_helper.get_parent_page_id(page_id)
 if parent_id:
     print(f"Parent page ID for page ID {page_id}: {parent_id}")
 else:
@@ -543,15 +547,15 @@
 Return:
 - `ID of the parent page` (str): If the specified page has a parent page, the method returns the ID of the parent page. This is useful for understanding the hierarchy of pages within Confluence spaces. 
 - `False`: If no parent page exists for the specified page or if there was an error in the fetch operation (such as an invalid page ID or a problem with the Confluence server), the method returns False. This helps to identify pages that are at the top level of their space or when an issue occurs with the retrieval process.
 ______________________________________________________________________________
 ## 12. Add Table of Content (TOC) in wiki page
 - Add a Table of Contents (TOC) to a Confluence wiki page if it doesn't already have one.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 result_message = wiki_helper.add_toc_to_page(page_id)
 print(result_message)
 ```
 Parameter
@@ -560,15 +564,15 @@
 Output and Return
 - The function returns a **message** indicating the operation's result. This could be a confirmation that the TOC was added successfully, a message stating that the TOC already exists, or an error message if the operation failed. 
 - **Error Handling**: If there are issues fetching the page data or updating the page, the function provides detailed error messages including the status code and response text from Confluence's API. This is helpful for diagnosing problems with the operation.
 ______________________________________________________________________________
 ## 13. Add row to the existing table in wiki page (beta)
 - Pass the header to identify the table and then add the row to that identified table
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 page_id = "123456"  # Example page ID
 headers = ["Header1", "Header2", "Header3"]  # The headers of the table you're targeting
 row_data = ["Data1", "Data2", "Data3"]  # The data for the new row
 
 result_message = wiki_helper.add_row_to_table(page_id, headers, row_data)
 print(result_message)
 ```
@@ -580,15 +584,15 @@
 Output and Return
 - The function returns a message indicating the result of the operation. This could be a confirmation of successful row addition, or an error message detailing why the operation failed.
 
 ______________________________________________________________________________
 ## 14. Add/Update row to the existing table in wiki page (beta)
 - Pass the header to identify the table and then add/update the row to that identified table
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 headers = ["Cluster Name", "Component Name", "Next Version"]  # The headers of your table
 new_row_data = ["Cluster1", "ComponentA", "v2.0"]  # Data for the new or updated row
 
 result_message = wiki_helper.update_or_add_table_row(page_id, headers, new_row_data)
 print(result_message)
@@ -602,14 +606,22 @@
 ______________________________________________________________________________
 # Data Privacy Note
 
 🔒 **We respect your privacy**: This module does **not** store any of your data anywhere. It simply interacts with the Atlassian Jira API to perform the requested operations. Ensure you manage your connection details securely.
 
 # Release Notes
 
+## Latest Release: 0.4.1 (28 May 2024)
+- Revision in documentation for better understanding
+  - Based on the internal design now `JIRA_URL`, `CONFLUENCE_URL` is replaced with `ATLASSIAN_URL`
+  - Technically we are using `https://domain.atlassian.net` only to address Jira and Wiki both
+  - This is mentioned in the top of the document as well
+- Beta Features (Continued from previous release):
+  - Beta functions `wiki_helper.add_row_to_table` & `wiki_helper.update_or_add_table_row` for improved table management.
+
 ## Latest Release: 0.4 (21 Mar 2024)
 - New Features:
   - JIRA Integration Enhancements:
     - Custom Ticket Creation: The `create_custom_ticket` function has been introduced, allowing for more flexible ticket creation in JIRA projects. This function supports additional fields, enabling users to specify custom data during ticket creation. 
     - Ticket Field Updates: The `update_ticket_with_fields` method has been added, offering the ability to update existing tickets with new or modified fields. This feature is crucial for maintaining accurate and up-to-date ticket information.
 - Beta Features (Continued from previous release):
   - Beta functions `wiki_helper.add_row_to_table` & `wiki_helper.update_or_add_table_row` for improved table management.
```

### Comparing `atlassian_modules-0.4/atlassian_modules/helper.py` & `atlassian_modules-0.4.1/atlassian_modules/helper.py`

 * *Files identical despite different names*

### Comparing `atlassian_modules-0.4/atlassian_modules.egg-info/PKG-INFO` & `atlassian_modules-0.4.1/atlassian_modules.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 Metadata-Version: 2.1
 Name: atlassian-modules
-Version: 0.4
-Summary: Modules for interacting with Atlassian products.
+Version: 0.4.1
+Summary: Modules for interacting with Atlassian cloud products.
 Home-page: 
 Author: Pavan Bhatt
 Author-email: pavanhbhatt1@gmail.com
 Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
 
 The best way to interact with Atlassian Jira/Confluence API.
 
+> **Note:** _This module is useful for the Atlassian Cloud_ <br>
+> Your URL should look like this https://domain.atlassian.net
+
+
 # Prerequisites
 ```python
 from atlassian_modules import JiraHelper # for Jira
 from atlassian_modules import  WikiHelper # for Wiki
 ```
 
 # Getting Started
 
 ## Connectivity to Atlassian Jira
 
 To initialize a connection to Jira, instantiate the `JiraHelper` class with your Jira URL, email, and API token:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 ```
 ______________________________________________________________________________
 ______________________________________________________________________________
 # Atlassian Jira
 ______________________________________________________________________________
 ______________________________________________________________________________
 ## 1. Create a Jira Ticket
 
 - You can create a new Jira ticket using the `create_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_url = jira_helper.create_ticket("PRJ", "Issue Summary", "Detailed issue description.", "Bug")
 if ticket_url:
     print(f"Ticket created: {ticket_url}")
 else:
     print("Failed to create ticket.")
 ```
@@ -56,15 +62,15 @@
 - `URL of the created ticket (str)`: If the ticket creation is successful, the function returns the URL to access the newly created ticket directly. 
 - `False`: If the ticket creation fails (for example, due to incorrect input parameters or server errors), the function returns `False`.
 ______________________________________________________________________________
 ## 2. Create a custom Jira Ticket
 - You can create a new custom Jira ticket using the `create_custom_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 # Define additional fields if necessary
 additional_fields = {
     "customfield_12345": "Custom value",
     "labels": ["label1", "label2"]
 }
 
@@ -88,15 +94,15 @@
 Return:
 - `URL of the created ticket` (str): If the ticket creation is successful, the function returns the URL to access the newly created ticket directly. This allows for immediate navigation to the ticket for review or further action.
 - `False`: If the ticket creation process fails, whether due to incorrect input parameters, server errors, or issues with the additional fields, the function returns `False`. This indicates that the ticket was not created and provides an opportunity to address any issues before retrying.
 ______________________________________________________________________________
 ## 3. Update the Jira ticket with inbuilt and custom fields
 - You can update any custom field of Jira ticket using the `update_ticket_with_fields` method:
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 # Define the additional fields you want to update
 additional_fields = {
     "customfield_12345": "New custom value",
     "labels": ["newlabel1", "newlabel2"]
 }
 
@@ -118,15 +124,15 @@
 - `False` otherwise. If the ticket update fails (for example, due to incorrect ticket ID, fields that cannot be updated, or server errors), the function returns `False`, and additional error information is printed to help diagnose the issue.
 ______________________________________________________________________________
 ## 3. Delete a Jira Ticket
 
 - To delete a ticket, use the `delete_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 if jira_helper.delete_ticket(ticket_key):
     print("Ticket deleted successfully.")
 else:
     print("Failed to delete ticket or ticket does not exist.")
 ```
@@ -139,15 +145,15 @@
 Return:
 - `True`: If the ticket is successfully deleted. This is indicated by a `204` HTTP status code from the JIRA API, meaning "`No Content`" but signifying successful deletion. 
 - `False`: If the deletion fails, which can occur if the ticket does not exist or if there's an issue with the API request (e.g., permissions, invalid ticket key). This is communicated by returning `False`.
 ______________________________________________________________________________
 ## 4. Get Transition ID
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 transition_name = "Close"
 transition_id = jira_helper.get_transitions(ticket_key, transition_name)
 if transition_id:
     print(f"Transition ID for '{transition_name}' is {transition_id}.")
 else:
@@ -166,15 +172,15 @@
 - `False`: If the specified transition is not found for the ticket, or if there is any failure in fetching transitions (e.g., due to an invalid ticket key, network issues, or server errors), the function returns `False`.
 ______________________________________________________________________________
 ## 5. Transition a Jira Ticket
 
 - To transition a ticket to a different status, use the `transition_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 transition_input = "Done"  # Can be a transition name like 'Done' or an ID like '31'
 if jira_helper.transition_ticket(ticket_key, transition_input):
     print("Ticket transitioned successfully.")
 else:
     print("Failed to transition ticket.")
@@ -193,15 +199,15 @@
 
 ______________________________________________________________________________
 ## 6. If exist a Jira Ticket
 
 - To check if a ticket exist, use the `if_ticket_exist` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 if jira_helper.if_ticket_exist(ticket_key):
     print("The ticket exists.")
 else:
     print("The ticket does not exist.")
 ```
@@ -216,15 +222,15 @@
 - `False`: If the ticket does not exist or if there was an error in checking. A `404` HTTP status code indicates the ticket does not exist. Other status codes indicate a failure in the request to check the ticket.
 ______________________________________________________________________________
 ## 7. Comment on a Jira ticket
 
 - To comment on the ticket, use the `comment_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 ticket_key = "PRJ-123"  # Example ticket key
 comment_text = "This is an example comment."
 comment_url = jira_helper.comment_ticket(ticket_key, comment_text)
 if comment_url:
     print(f"Comment added successfully: {comment_url}")
 else:
@@ -242,15 +248,15 @@
 - `False`: If adding the comment fails. This could be because the ticket does not exist, the comment text is invalid, or there was an error in the request itself. In such cases, the function returns `False`.
 ______________________________________________________________________________
 ## 8. Pass the JQL and get the ticket array
 
 - To query tickets using JQL, use the `jql_ticket` method:
 
 ```python
-jira_helper = JiraHelper(JIRA_URL, EMAIL, API_TOKEN)
+jira_helper = JiraHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 jql_query = "project = PRJ AND status = 'Open'"
 max_results = 100  # Optional
 ticket_keys = jira_helper.jql_ticket(jql_query, max_results)
 if ticket_keys:
     print(f"Found tickets: {', '.join(ticket_keys)}")
 else:
@@ -271,15 +277,15 @@
 ______________________________________________________________________________
 # Atlassian Wiki
 ______________________________________________________________________________
 ______________________________________________________________________________
 ## 1. Creating a wiki page
 - To create wiki page, use the `create_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(CONFLUENCE_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 space_key = "DEV"
 title = "API Documentation"
 content = "<p>This is the API documentation for our project.</p>"
 parent_page_id = 123456  # Optional
 page_url = wiki_helper.create_wiki_page(space_key, title, content, parent_page_id)
 if page_url:
@@ -299,15 +305,15 @@
 Return: 
 - `URL of the created Confluence page` (str): If the page creation is successful, the function returns the URL to access the newly created page. This is indicated by a `200` HTTP status code. 
 - `False`: If the page creation fails. This could be due to various issues, such as invalid input parameters, permissions problems, or server errors. In such cases, the function returns `False`.
 ______________________________________________________________________________
 ## 2. Duplicate a wiki page
 - To duplicate wiki page, use the `duplicate_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 source_page_id = "12345"  # Example source page ID
 target_space_key = "TGT"  # Example target space key
 target_title = "Duplicated Page Title"  # New title for the duplicated page
 target_parent_page_id = "67890"  # Optional parent page ID for the new page
 
 duplicated_page_url = wiki_helper.duplicate_wiki_page(source_page_id, target_space_key, target_title, target_parent_page_id)
@@ -327,15 +333,15 @@
 Return: 
 - `URL of the duplicated Confluence page` (str): If the duplication is successful, the method returns the URL to access the newly created duplicated page. This URL is constructed from the response of the page creation process. 
 - `None`: If the duplication fails at any point (e.g., retrieving content from the source page, creating the new page), the method returns `None`. This indicates that the operation was not successful, and no new page was created.
 ______________________________________________________________________________
 ## 3. Create a wiki page from template
 - To create a wiki page from template use the `create_page_from_template` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 template_id = "12345"  # Example template ID
 space_key = "TGT"  # Example space key
 title = "New Page from Template"  # Title for the new page
 parent_page_id = "67890"  # Optional parent page ID
 
 created_page_url = wiki_helper.create_page_from_template(template_id, space_key, title, parent_page_id)
@@ -354,15 +360,15 @@
 Return: 
 - `URL of the created Confluence page` (str): If the page creation is successful, the function returns the URL to access the newly created page. This indicates that the page was created successfully and is accessible at the returned URL. 
 - `None` or `False`: If the page creation fails, due to reasons such as template retrieval failure, duplicate title, or any error in the creation process, the function returns `None` or `False`. This indicates that no new page was created.
 ______________________________________________________________________________
 ## 4. Move wiki page from one location to another
 - To move wiki page from one location to another location without changing title use `move_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "12345"  # Example page ID to be moved
 target_space_key = "NEWSPACE"  # Target space key
 target_position = "append"  # Position of the page relative to the parent page ('append', 'above', 'below')
 target_parent_page_id = "67890"  # Optional new parent page ID
 
 moved_page_url = wiki_helper.move_wiki_page(page_id, target_space_key, target_position, target_parent_page_id)
@@ -381,15 +387,15 @@
 Return: 
 - `URL of the moved Confluence page` (str): If the move operation is successful, the function returns the URL to access the moved page. This indicates that the page was successfully moved to the new space and position. 
 - `None` or `False`: If the move operation fails, due to reasons such as an error retrieving the current page details, an error in the move operation, or inability to retrieve the moved page URL, the function returns `None` or `False`. This indicates that the page was not successfully moved.
 ______________________________________________________________________________
 ## 5. Check if wiki page exist
 - To move wiki page from one location to another location without changing title use `move_wiki_page` method:
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 title = "Example Page Title"  # Title of the Confluence wiki page to check
 space_key = "EX"  # Key of the Confluence space
 
 if wiki_helper.wiki_page_exists(title, space_key):
     print(f"The page '{title}' exists in space '{space_key}'.")
 else:
@@ -403,15 +409,15 @@
 Return: 
 - `True`: If the page exists. This is determined by the presence of results matching the specified title in the specified space. 
 - `False`: If the page does not exist or if there was an error during the request. This could be due to the specified page not being found in the given space or an issue with the Confluence API response.
 ______________________________________________________________________________
 ## 6. Retrieve all child pages
 - Recursively retrieve all descendant pages of a given parent page ID.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 parent_id = "12345"  # Example parent page ID
 child_pages = wiki_helper.get_child_pages_recursive(parent_id)
 if child_pages:
     print("Child pages found:")
     for page in child_pages:
         print(f"Title: {page['title']}, ID: {page['id']}, Parent ID: {page['parentid']}")
@@ -428,15 +434,15 @@
 Return: 
 - `List of child pages`: Returns a list of dictionaries, each containing the title, ID, and parent ID of each descendant page found. This allows for a comprehensive view of the hierarchy and content under the specified parent page. 
 - If the retrieval fails at any point (due to an error in fetching child pages, for instance), the recursive fetching process is designed to continue for other branches of the tree, aiming to return as complete a list as possible of descendant pages.
 ______________________________________________________________________________
 ## 7. Get wiki page ID
 - Retrieve the ID of a Confluence wiki page by its title.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 title = "Example Page"  # Title of the Confluence wiki page to search for
 space_key = "EX"  # Key of the Confluence space
 
 page_id = wiki_helper.get_page_id(title, space_key)
 if page_id:
     print(f"Found page '{title}' with ID: {page_id} in space '{space_key}'.")
@@ -455,15 +461,15 @@
 Return:
 - `ID of the page` (str): If a page with the specified title is found in the given space, the function returns the ID of the page. 
 - `False`: If no page is found with the given title in the specified space, or if there was an error during the request, the function returns `False`.
 ______________________________________________________________________________
 ## 8. Replace word in wiki
 - Replace all occurrences of a string in a Confluence wiki page.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 from_string = "old text"  # Text to be replaced
 to_string = "new text"  # Replacement text
 
 if wiki_helper.replace_in_page(page_id, from_string, to_string):
     print(f"Replaced all occurrences of '{from_string}' with '{to_string}' in page ID: {page_id}.")
@@ -483,15 +489,15 @@
 Return:
 - `True`: If the replacement operation was successful, whether replacements were made or not (including the case where the `from_string` was not found). 
 - `False`: If there was a failure at any point during the process, such as an error fetching the page content, or updating the page with the new content.
 ______________________________________________________________________________
 ## 9. Fetch tables from wiki
 - Fetch all tables from a Confluence wiki page.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 tables_json = wiki_helper.get_tables_from_page(page_id)
 if tables_json:
     print("Found tables on the page:")
     print(tables_json)
@@ -506,15 +512,15 @@
 Return:
 - JSON structure: Returns a JSON string that represents all the tables found on the page. Each table is structured into a JSON object with keys representing the table headers and values representing the row data. If multiple tables are found, they are indexed as `table1`, `table2`, etc., in the JSON structure. 
 - If the fetching fails (due to an unsuccessful API call) or if no tables are found on the page, the function returns an empty JSON object (`{}`).
 ______________________________________________________________________________
 ## 10. Replace the whole wiki page
 - Replace the entire Confluence wiki page with the new content
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "12345"  # Example page ID
 new_content = "<p>This is the new content for the page.</p>"  # HTML content
 
 if wiki_helper.update_wiki_page(page_id, new_content):
     print(f"Page ID: {page_id} was updated successfully.")
 else:
@@ -529,15 +535,15 @@
 Return:
 - `True`: If the page content update is successful. This is indicated by a status code of `200` from the Confluence REST API, showing that the update request was processed correctly. 
 - `False`: If the update fails. This could be due to various reasons such as an invalid page ID, issues with the Confluence server, or improper formatting of the new content. Failure is indicated by any status code other than `200`, and the method prints the error details received from the server.
 ______________________________________________________________________________
 ## 11. Get parent page ID
 - Retrieve the parent ID of a Confluence wiki page by passed page ID.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 parent_id = wiki_helper.get_parent_page_id(page_id)
 if parent_id:
     print(f"Parent page ID for page ID {page_id}: {parent_id}")
 else:
@@ -552,15 +558,15 @@
 Return:
 - `ID of the parent page` (str): If the specified page has a parent page, the method returns the ID of the parent page. This is useful for understanding the hierarchy of pages within Confluence spaces. 
 - `False`: If no parent page exists for the specified page or if there was an error in the fetch operation (such as an invalid page ID or a problem with the Confluence server), the method returns False. This helps to identify pages that are at the top level of their space or when an issue occurs with the retrieval process.
 ______________________________________________________________________________
 ## 12. Add Table of Content (TOC) in wiki page
 - Add a Table of Contents (TOC) to a Confluence wiki page if it doesn't already have one.
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 
 result_message = wiki_helper.add_toc_to_page(page_id)
 print(result_message)
 ```
 Parameter
@@ -569,15 +575,15 @@
 Output and Return
 - The function returns a **message** indicating the operation's result. This could be a confirmation that the TOC was added successfully, a message stating that the TOC already exists, or an error message if the operation failed. 
 - **Error Handling**: If there are issues fetching the page data or updating the page, the function provides detailed error messages including the status code and response text from Confluence's API. This is helpful for diagnosing problems with the operation.
 ______________________________________________________________________________
 ## 13. Add row to the existing table in wiki page (beta)
 - Pass the header to identify the table and then add the row to that identified table
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 page_id = "123456"  # Example page ID
 headers = ["Header1", "Header2", "Header3"]  # The headers of the table you're targeting
 row_data = ["Data1", "Data2", "Data3"]  # The data for the new row
 
 result_message = wiki_helper.add_row_to_table(page_id, headers, row_data)
 print(result_message)
 ```
@@ -589,15 +595,15 @@
 Output and Return
 - The function returns a message indicating the result of the operation. This could be a confirmation of successful row addition, or an error message detailing why the operation failed.
 
 ______________________________________________________________________________
 ## 14. Add/Update row to the existing table in wiki page (beta)
 - Pass the header to identify the table and then add/update the row to that identified table
 ```python
-wiki_helper = WikiHelper(JIRA_URL, EMAIL, API_TOKEN)
+wiki_helper = WikiHelper(ATLASSIAN_URL, EMAIL, API_TOKEN)
 
 page_id = "123456"  # Example page ID
 headers = ["Cluster Name", "Component Name", "Next Version"]  # The headers of your table
 new_row_data = ["Cluster1", "ComponentA", "v2.0"]  # Data for the new or updated row
 
 result_message = wiki_helper.update_or_add_table_row(page_id, headers, new_row_data)
 print(result_message)
@@ -611,14 +617,22 @@
 ______________________________________________________________________________
 # Data Privacy Note
 
 🔒 **We respect your privacy**: This module does **not** store any of your data anywhere. It simply interacts with the Atlassian Jira API to perform the requested operations. Ensure you manage your connection details securely.
 
 # Release Notes
 
+## Latest Release: 0.4.1 (28 May 2024)
+- Revision in documentation for better understanding
+  - Based on the internal design now `JIRA_URL`, `CONFLUENCE_URL` is replaced with `ATLASSIAN_URL`
+  - Technically we are using `https://domain.atlassian.net` only to address Jira and Wiki both
+  - This is mentioned in the top of the document as well
+- Beta Features (Continued from previous release):
+  - Beta functions `wiki_helper.add_row_to_table` & `wiki_helper.update_or_add_table_row` for improved table management.
+
 ## Latest Release: 0.4 (21 Mar 2024)
 - New Features:
   - JIRA Integration Enhancements:
     - Custom Ticket Creation: The `create_custom_ticket` function has been introduced, allowing for more flexible ticket creation in JIRA projects. This function supports additional fields, enabling users to specify custom data during ticket creation. 
     - Ticket Field Updates: The `update_ticket_with_fields` method has been added, offering the ability to update existing tickets with new or modified fields. This feature is crucial for maintaining accurate and up-to-date ticket information.
 - Beta Features (Continued from previous release):
   - Beta functions `wiki_helper.add_row_to_table` & `wiki_helper.update_or_add_table_row` for improved table management.
```

