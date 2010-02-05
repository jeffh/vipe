# Test Server

This was borne out of frustration with the current state of DRB, autospec / test
/ rspactor et al. They were just taking too long to set up for me.

I'd like to run tests with DRB, but it seems that's currently broken in
rspec-rails (fix not gemmed up yet).

Maybe someone else can use this as a base for their own particular solution. You
can use this approach to do anything you like with the file you're currently
editing, or anything you like with whatever you throw at the named pipe.

## Installation

* Run test_server.rb in a terminal
* Copy test_client.vim to ~/.vim/plugin/
* Fire up Vim and open a spec or feature file.
* Type ':call RunTest()' or ':call RunExample()' for example under line
* ???
* Eat flapjacks

I recommend binding functions to keys, for example:

    map <F12> :w<CR>:call RunTest()<CR>
    imap <F12> <ESC>:w<CR>:call RunTest()<CR>
    map <F11> :w<CR>:call RunExample()<CR>
    imap <F11> <ESC>:w<CR>:call RunExample()<CR>

In your ~/.vimrc will bind F12 to save-and-run-test and F11 to
save-and-run-example
