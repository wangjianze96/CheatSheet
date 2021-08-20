# CheatSheet for Vim

This cheatsheet only contains the instructions that I use frequently,
for more info, go check [this website](https://vim.rtorr.com/)

## Movement
`G`				// go to the bottom of a file          
`gg`			// go to the top of a file           
`w`				// jump forwards to the start of a word, can add number before it       
`W`				// jump forwards to the start of a word (words can contain punctuation)             
`b`				// jump backwards to the start of a word              
`B`             
`e`				// jump forwards to the end of a word            
`E`         
`ge`			// jump backwards to the end of a word          
`gE`		
`0`				// jump to the start of a line           
`$`				// jump to the end of the line            
`:lineNumber`	// go to a certain line

## Insert mode
`o`				// append (open) a new line below current line          
`O`				// append (open) a new line above current line               
`Ctrl+rx`		// insert the contents of register x           

## Editing
`u`				// undo          
`U`				// restore (undo) last changed line     
`Ctrl+r`		// redo
`.`				// repeat last command          
`yy`			// yank (copy) a line        
`2yy`			// yank (copy) 2 lines       
`yw`			// yank (copy) the characters of the word from the cursor position to the start of the next word       
`yiw`			// yank (copy) word under the cursor       
`yaw`			// yank (copy) word under the cursor and the space after or before it          
`y$`			// yank (copy) to end of line          
`p`				// put (paste) the clipboard after cursor         
`P`				// put (paste) before cursor       
`dd`			// delete (cut) a line      
`2dd`			// delete (cut) 2 lines       
`dw`			// delete (cut) the characters of the word from the cursor position to the start of the next word             
`diw`			// delete (cut) word under the cursor       
`daw`			// delete (cut) word under the cursor and the space after or before it          
`D`				// delete (cut) to the end of the line
`d$`			// delete (cut) to the end of the line            
`x`				// delete (cut) character

### Indent Text
`>>`			// indent (move right) line one shiftwidth        
`<<`			// de-indent          
`>%`			// indent a block with () or {} (cursor on brace)        
`>ib`			// indent inner block with ()
`>at`			// indent a block with <> tags           
`3==`			// re-indent 3 lines         
`=%`			// re-indent a block with () or {}                 
`gg=G`			// re-indent entire buffer       

### Visual Mode
`v`				// start visual mode          
`V`				// start linewise visual mode            
`o`				// (in visual mode) move to other end of marked area    
`Ctrl+v`		// start visual block mode          
`O`				// (in visual block mode) move to other corner of block        
`aw`			// mark a word       

### Visual Commands
`>`				// shift text right         
`<`				// shift text left              
`y`				// yank (copy) marked text          
`d`				// delete marked text         
`~`				// switch case        
`u`				// change marked text to lowercase    
`U`				// change marked text to uppercase       

## Register
`:reg`			// show register content           
`"xy`			// yank into register x          
`"xp`			// paste contents of regitser x  
`"+y`			// yank into the system clipboard register      
`"+p`			// paste from the system clipboard register        

## Macros
`qa`			// record macro a         
`q`				// stop recording macro          
`@a`			// run macro a        
`@@`			// rerun last run macro          

## Search and Replace
`/pattern`		// search for patten          
`?pattern`		// search backward for pattern         
`\vpattern`		// for non-alphanumeric characters        
`n`				// repeat search in same direction           
`N`				// repeat search in opposite direction     
`:%s/old/new/g`	// replace all old with new throughout file         
`:%s/old/new/gc`// replace all old with new throughout file with confirmations       
`:noh[lsearch]`	// remove highlighting of search matches
