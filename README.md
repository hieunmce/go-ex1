# Library API excercise

**Library API excercise** is a golang implement of library API

Submitted by: **{{github_user_name}}**

Time spent: **{{time_spent}}** hours spent in total

## User Stories

### Required:

#### Stage 1:
* [ ] API must be able to CRUD category of books:
  * [ ] Each category should have the following fields:
    * name (string)
    * tags (string)
  * [ ] API must be able to get detail of a category.
  * [ ] API must be able to get list of categories.
  * [ ] API must be able to create a category.
  * [ ] API must be able to update a category.
  * [ ] API must be able to delete a category.
  * [ ] when delete categories all book belongs to that categories should deleted too.
  
* [ ] Validate category is correct before (Create/Update):
  * [ ] validate name of category is not empty and length > 5 characters.
  * [ ] validate name of category not existed yet (for both create and update).

* [ ] API must be able to CRUD books:
  * [ ] Each book should have the following fields:
    * name (string)
    * category_id
    * author (string)
    * description (string)
    * tags (string)
  * [ ] API must be able to get detail of a book.
  * [ ] API must be able to get list of books.
  * [ ] API must be able to create a book.
  * [ ] API must be able to update a book.
  * [ ] API must be able to delete a book.
  
* [ ] Validate books is correct before (Create/Update):
  * [ ] validate category of a book is exist, if not reject it with error message
  * [ ] validate name of a book is not empty and length > 5 characters. if not reject it with error message
  * [ ] validate description of a book is not empty and length > 5 characters. if not reject it with error message
  
* [ ] API must be able to CRUD users:
  * [ ] Each user should have the following fields:
    * name (string)
    * emails (string)
  * [ ] API must be able to get list of users
  * [ ] API must be able to create a user
  * [ ] API must be able to update a user
  * [ ] API must be able to delete a user
  
#### Stage 2:
* [ ] API must be able to make action: user lend a book:
  * [ ] API should have the following fields:
    * book_id
    * user_id
    * from (datetime)
    * to (datetime)
  * [ ] validate books is available to lend, if not available reject with error message
  * [ ] validate 1 user only can lend 3 books, if lend more reject with error message
  
* [ ] API must be able to get current user who lending that book

* [ ] API must be able to make action: user return a book:
  * [ ] API should have the following fields:
    * book_id
    * user_id
    * return_date (datetime)
  * [ ] validate books is available to return(user_id is current who lending that book), if not available reject with error message.
  
* [ ] API must be able to gets list of books and it status (virtual base by lending status)
  
* [ ] When user or book get deleted, also remove relation (lends, returns** between users and books.

### Optional:

*  [ ] List books and filter by names, availables
*  [ ] batch create books (create multiple book with 1 API)
*  [ ] batch lending books (user can lending multiple books with 1 api)
*  [ ] batch return books (user can return multiple books with 1 api)
*  [ ] implement feature add a tags to books can search book by tag name


The following **additional** features are implemented:

* [ ] .....

The following **known issues**:

* ...

## Video Walkthrough

Here's a walkthrough of implemented user stories:


## Notes

Notes about current git.

## License

    Copyright [2016] [{{github_user_name}}]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
