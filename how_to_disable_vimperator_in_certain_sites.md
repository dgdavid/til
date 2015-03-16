I needed to disable [Vimperator](http://www.vimperator.org/vimperator) in certain sites, as for example in my email web client.

I found the [solution](http://stackoverflow.com/questions/14271624/disable-vimperator-temporarily) in StackOverflow :D

In short, adds to  `~/.vimperatorrc`

```
autocmd LocationChange .*                        js modes.passAllKeys = false
autocmd LocationChange address\\.certain\\.site  js.modes.passAllKeys = true
```
