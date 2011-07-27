Syntax Highlighting for Genshi Text Templates in Vim
----------------------------------------------------

In order to add syntax highlighting for Genshi_ `text templates`_ to Vim_,
move the `genshi.vim`_ file into the ``~/.vim/syntax/`` directory.  If your
text templates have a ``.genshi`` file extension (and your `XML templates`_
don't), you could add the following lines to your ``~/.vim/filetype.vim`` in
order to auto-detect them::

  augroup filetypedetect
    autocmd BufNewFile,BufRead *.genshi setfiletype genshi
  augroup END

.. References

.. _Vim:
   http://www.vim.org/
.. _Genshi:
   http://genshi.edgewall.org/
.. _XML templates:
   http://genshi.edgewall.org/wiki/Documentation/xml-templates.html
.. _text templates:
   http://genshi.edgewall.org/wiki/Documentation/text-templates.html
.. _genshi.vim:
   https://raw.github.com/weiss/genshi.vim/master/genshi.vim
