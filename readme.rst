Jirafs-Graphviz
===============

Automatically converts graphviz (dot) you enter into your Jira comment
or description before uploading to JIRA.

Use
---

You can enter a digraph into your document by using the ``graphviz`` macro::

   <jirafs:graphviz>
      digraph {
         a -> b;
      }
   </jirafs:graphviz>

Upon submission to Jira, a file will automatically be generated, and your markup will be replaced with an embedded image showing your rendered digraph.

Installation
------------

1. Install from PIP::

    pip install jirafs-graphviz

2. Enable for a ticket folder::

    jirafs plugins --enable=graphviz

Note that you can globally enable this (or any) plugin by adding the
``--global`` flag to the above command::

    jirafs plugins --global --enable=graphviz

Requirements
------------

* Graphviz
