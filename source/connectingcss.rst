Connecting CSS styles
=====================
.. raw:: html

    <style type="text/css"">
        .red {
            color: red
        }
    </style>

 
The next line is of red color.

.. rst-class:: red

    This line text has red color

This effect has been obtained by using two directives: `raw
<http://docutils.sourceforge.net/docs/ref/rst/directives.html#raw-data-pass-through>`_ and `rst-class` or `class
<http://docutils.sourceforge.net/docs/ref/rst/directives.html#class>`_. By `raw
<http://docutils.sourceforge.net/docs/ref/rst/directives.html#raw-data-pass-through>`_ directive we inject the css
styles

.. code-block:: none

    .. raw:: html

        <style type="text/css"">
            .red {
                color: red
            }
        </style>

The `rst-class` is used to add the suitable class to next element. In our case it is the next paragraph.

.. code-block:: none

    .. rst-class:: red

        This line text has red color


Let gather all pieces together. The red line should be implemented by the code

.. code-block:: none

    .. raw:: html

        <style type="text/css"">
            .red {
                color: red
            }
        </style>

    .. rst-class:: red

        This line text has red color

