# Coconut Script
The home of Coconut Script.
AKA Colon Script.
Still in development, and still working on a compiler, but here's what it looks like:
Coconut Script is inspired by C++ and scratch.mit.edu
# General Info
Here is some general info.
This coding language does not use parentheses. Actually the text inside of a parentheses is a comment.
It uses colons and curly brackets. Practically nothing else. Most scripts do what they're called too.
# Sample code
start:coconut:0:1 (startup script, coconut v 0.1
var:time (global variables declared here)
sprite:cursor {
	insert:image:button.png
	on:start {
		pos:x::0:y::0
		costume::1
		time::0 (if there is no operator in between the colons, it is automatically referred to =)
		forever { 
			time:+=:0.01
			if:time:>:0.5 {
				dir:tow:[mouse:x]:[mouse:y]
				mv:[[distance:mouse]/5]
			}
			if:touching:edge {
				while:[touching:edge] {
					mv:-5 }
				time::0
				repeat:5 {
					mv:-2 }
			}
		}
	}
}
