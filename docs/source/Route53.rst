Route53
=======

.. raw:: html

    <style type="text/css">
          .gist .blob-wrapper.data {
             max-height:200px;
             bgcolor: #333333;
                overflow:auto;
                }
    </style>
    
A missing piece of Route53 is the ability to easily delete a hosted zone. In order to delete a hosted zone one must first delete all of the assiciated resource records.  While there is some anti-oops security to this, it's a real pain when you have lots of things to delete or want to delete things quickly as part of your workflow. Here follows a python/boto2 function for deleting a zone by name.


.. gist:: https://gist.github.com/jerm/5207d57a1077420f2bc9

