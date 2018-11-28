# Glossary  

Although most are general terms, it is still good to standardise the terminology to clear confusion just in case.
* Forum: our beloved cs1010s has different forums: General Discussion, Trainings, Recitation & Tutorials...
* Topic/thread: inside each forum, there are many topics related to that forum's main theme of discussion.
* Post: inside each topic, there are multiple posts. And this is what we will assign the class labels to.
Label/class label/classification...: the categories which posts can fall under


# Dataset Format  

#### About saving the post contents
* Each post has a numerical id as the primary key. When storing files related to the post, use that id as the prefix.
* Each post should have only 1 textual content file, name that file as "<post id>-text".
* Each post may have picture file(s), name the file(s): "<post id>-pic1.<pic format>", "<post id>-pic2.<pic format>", ...
* If a post has other file(s), name the file(s): "<post id>-other1.<file format>", "<post id>-other2.<file format>", ...  

#### About saving post, topic link, user, and label mappings
This information is saved in comma-separated csv file.
The csv file has the following columns, data types and relationships:  

|Column Name | Data Type | Remarks
| :---: | :---: | :---: |
| post_id | integer |  |
| username | string |  |
| topic_link | string |  |
| burnt_rice | binary | indicate here if any label is a subset of or complementary to of another |
| brown_rice | binary |  |
| rice | binary |  |
| vegetable | binary |  |
| meat | binary |  |
| meat+ | binary |  |
| fish | binary |  |

#### Examples
Refer to *sample-dataset*.  
