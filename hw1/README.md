# HW01: Text Editor Tutorials

Name: <your name here>
Course: <this course name>

## Vim

#### Question 1
What is the configuration file for Vim? What are the minimal changes to this configuration to allow for syntax highlighting and tab management for Python?

vimrc (vim resource configuration) file. Enable syntax highlighting, show line numbers, set tabs to have 4 spaces, indent when moving to the next line while writing code, expand tabs into spaces, when using the >> or << commands, shift lines by 4 spaces, show a visual line under the cursor's current line, show the matching part of the pair for [] {} and (), enable all Python syntax highlighting features.

#### Question 2
What is the best/most popular way to extentend Vim? Does Vim have a "plugin" system?

One popular way to extended vim is Vim bundle (Vundle). Vundle allows you to keep track of and configure your plugins right in the vimrc install configured plugins update configured plugins. Vim does have a plugin system. 

#### Question 3
What are the most popular Vim extensions for Python development? Use your favorite search engine to find out more about how to use Vim to edit and work with Python code.

Popular Vim extensions:
fugitive.vim, syntastic, vim-gitgutter 

## Emacs

#### Question 1
What is the configuration file for Emacs? Find some example Emacs configuration files, especially ones that deal with Python development, and provide links to them.

~/. emacs, d/init. el.
https://www.gnu.org/software/emacs/manual/html_node/efaq-w32/Location-of-init-file.html
http://pragmaticemacs.com/emacs/editing-your-emacs-config-file/

#### Question 2
What is the best/most popular way to extentend Emacs? Does Emacs have a "plugin" system?

One popular way is Magit. Emacs does have a plugin system. 

#### Question 3
What are the most popular Emacs extensions for Python development? Use your favorite search engine to find out more about how to use Emacs to edit and work with Python code.

The Elpy package and Flymake which is built in to Emacs.

