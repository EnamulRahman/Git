Repository :                a Git project (tracked folder with a .git directory) 

Commit :                        a snapshot of your files and metadata (author, timestamp, message, parent   commit, etc.) 

Branch :                          a movable pointer to a specific commit (e.g., main, dev, feature/login) 

Remote :                         a reference to an external Git host (like GitHub, GitLab) usually named origin 

Staging Area :            also called the Index; a buffer between your working directory and the repo what you plan to   

                                                     commit 

Blobs :                              “binary large object” — stores the actual content of files (just the data, no filename/path) 

Trees :                               stores filenames, file paths, and pointers to blobs (files) and other trees   (directories).  

                                                      Represents a directory snapshot 

Refs (Reference) :    pointer to a commit: branches (refs/heads), tags (refs/tags), and special ones  like HEAD 

HEAD :                              pointer to the current branch or commit you're working on 

Index :                              the actual file .git/index, a binary file that holds the staging area info 

Object Store :             .git/objects/ — where Git stores all blobs, trees, and commits by SHA hash 

Tag :                                    a ref to a specific commit, often used for marking releases 
