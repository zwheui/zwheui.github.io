### [Return to Readme](../README.md#rubysyntax)
### Notes Ruby Syntax
================
##### Don't learn ruby on windows (Chinese) [link](https://ruby-china.org/topics/1020)

* Youtube [link](https://www.youtube.com/watch?v=Dji9ALCgfpM)

* There is a trap of the multiline of the `,`

* We can easily run ruby command in the Mac terminal by create a *.rb file and run `ruby *.rb`

* We can also run `irb` in terminal, then we can run ruby command, input `exit` to back

* Syntax `copy the command below and replace * with space, then you can run them by ruby`
	* We can use `print` or `puts` to output the result on terminal
		* print "hello world\n"				# (No line break)
		* puts	'hello world'				# (With line break)
		* # Arithmetic Operators
		* # `+ - * / %`
		* puts	1.class
		* puts	1.234.class
		* puts  "A String".class

	* String can use single quote or double quote, but double quote will execute command such as "hello word\n"

	* CONSTANT is start from Upper case, CONSTANT can be update in ruby
		* A_constant = 11
		* A_constant = 12
		* puts A_constant

	* Create a file by command: `File`
		* a_file = File.new("file.txt", "w")
		* a_file.puts("blah\n blah").to_s
		* a_file.close
		* data_from_a_file = File.read("file.txt")
		* File.delete("file.txt")
		* puts data_from_a_file

	* Run another ruby file by using `load`
		* load "test1.rb"

	* Multiline Comment
		* =begin
		* blah blah blah
		* =end

	* Comparison : `== != < > <= >=`

	* Logical : `&& || ! and or not`
		* puts (true && false).to_s
		* puts (true || false).to_s
		* puts (!false).to_s
		* puts (true and false).to_s
		* puts (true or false).to_s

	* Special Comparison `<=>` only return -1 1 0
		* puts (5 <=> 10).to_s
		* puts (50 <=> 10).to_s
		* puts (10<=> 10).to_s

	* Keyword `unless`
		 * age = 55
		 * puts "You're Old 50" if age > 50
		 * puts "You're Old 60" unless age < 60

	* Keyword `gets.chomp` get user input in terminal

	* Keyword `case when when else end`
		* name = gets.chomp
		* case name
		* when "tom1","tom2"
		* 	puts "tom zhu"
		* 	exit
		* else
		* 	puts "not tom"
		* end

	* Keyword `? :`
		* puts (10 > 12) ? "true" : "false"

	* Keyword 'loop {next break}' `while x <= 10` `until x > 10` `for i in list`
		* x = 1
		* loop { 
		* 	x += 1
		* 	next unless (x % 2) == 0
		* 	puts x
		* 	break if x >= 10
		* }
		* myArrayList = [1,2,3,4,5]
		* myArrayList.each do |myArray|
		* 	puts "this is #{myArray.to_s}"
		* end
		* (0..10).each do |i|
		*	puts "No #{i.to_s}"
		* end

	* Keyword `def` for function/method
		* def fn_01(param01, param02)
		* 	return	puts param01.to_i + param02.to_i
		* end
		* puts fn_01(10, 20)

	* Any value change in the function won't impact the value declare out of the function
		* x = 1
		* def change_x(param)
		* 	param = 4
		* end
		* change_x(x)
		* puts "X = #{x}"

	* handle error `begin / rescue / else / ensure / end` [link](http://stackoverflow.com/questions/2191632/begin-rescue-and-ensure-in-ruby) like `try catch final` in the C#
		* begin
		*  # something which might raise an exception
		* rescue SomeExceptionClass => some_variable
		*   # code that deals with some exception
		* rescue SomeOtherException => some_other_variable
		*   # code that deals with some other exception
		* else
		*   # code that runs only if *no* exception was raised
		* ensure
		*   # ensure that this code always runs, no matter what
		* end

	* Keyword `raise ArgumentError`

	* Multiline by `<<EOM blah\n blah\n EOM`

	* Keyword `include? size count start_with? index`

	* Keyword `upcase downcase swapcase`

	* Keyword `lstrip rstrip strip`	like `trim` in c#

	* Keyword `rjust ljust center`
		* puts "abcd".center(10, '.')

	* Keyword `split(//) split(/ /) split(/,/)`

	* Escape sequences
		* # \\ Backslash
		* # \' Single-quote
		* # \" Double-quote
		* # \a Bell
		* # \b Backspace
		* # \f Formfeed
		* # \n Newline
		* # \r Carriage
		* # \t Tab
		* # \v Vertical Tab

#### Class

	* # Keyword on class property `attr_reader attr_writer attr_accessor`
		* class People
		*	attr_reader :name , :age, :height
		*	attr_writer :age
		*	attr_accessor :weight
		*	def speak_my_weight()
		*		puts "My weight is #{self.weight.to_s}"
		* 	end
		* end
		* tom = People.new
		* # tom.name = "Tom Zhu"
		* tom.weight = 150
		* puts tom.weight.to_s
		* tom.speak_my_weight()

	* # Keyword inherit class ` < `
		* class ChinesePeople < People
		*  	def speak_my_weight
		*  		puts "Chinese People say My weight is #{self.weight.to_s}"
		*   end
		* end

		* jerry = ChinesePeople.new
		* jerry.weight = 200
		* jerry.speak_my_weight

#### Module

	* # Keyword `require_relative "Module Name"` out of class
	* # Keyword `include` Module Name in the class
	* # Keyword `prepend` Module Name in the class

#### Symbole
	* :test
	* puts :test
	* puts :test.to_s
	* puts :test.class
	* puts :test.object_id





















