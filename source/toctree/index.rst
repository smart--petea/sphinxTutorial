Using The TOCTree directive
===========================

    Today we will explore an important feature of sphinx - the `toctree` markup construct.

    .. note::

        `toctree` can be decrypted as ` Table Of Contents tree`

    `toctree` command help to gather a bunch of files together. 

    My project has three files `Chapter1.rst`, `Chapter2.rst` and `Chapter3.rst`.

    **Chapter1.rst**

    .. code-block:: none

        Chapter1
        =============

    **Chapter2.rst**

    .. code-block:: none

        Chapter2
        =============

    **Chapter3.rst**

    .. code-block:: none

        Chapter3
        =============

    Let generate the table of contents `TOC` in the `index.rst`.

    **index.rst**

    .. code-block:: none

        **Table of Contents**

        .. toctree::

            Chapter1.rst
            Chapter2.rst
            Chapter3.rst


    Compile the project and stare at the result. You should have obtained something like next table of contents

    **Table of Contents**

    .. toctree::

        ch1.rst
        ch2.rst
        ch3.rst
    

    .. note::
        
        There are still rocks you can grind up. Read the official docs of `toctree
        <http://www.sphinx-doc.org/en/stable/markup/toctree.html#toctree-directive>`_. Be carefull at it's parameters
        `:numbered:`, `:maxdepth:` ... and your table of contents would be of a particular view.
    
