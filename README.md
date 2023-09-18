# Writing Good Documentation

## Step - 1 - Using Codeblocks.

Codeblocks in markdown make it *very easy* for tech people to **copy, paste, share** code.
A good _Cloud Engineer_ uses Codeblocks whenever possible.

Because it allows other to copy and paste heir code to replicate or research issues.

- In order to create codeblocks in markdown you need to use three backticks (`)
- Not to be confused with quotation (')

```
def factorial(n)
  if n == 0
    return 1
  else
    return n * factorial(n - 1)
  end
end

# Test the factorial function
puts "Enter a number to calculate its factorial:"
number = gets.chomp.to_i

if number < 0
  puts "Factorial is not defined for negative numbers."
else
  result = factorial(number)
  puts "The factorial of #{number} is #{result}."
end
```


- When you can you should attempt to apply syntax highlighting to your codeblocks

 ```ruby
def factorial(n)
  if n == 0
    return 1
  else
    return n * factorial(n - 1)
  end
end

# Test the factorial function
puts "Enter a number to calculate its factorial:"
number = gets.chomp.to_i

if number < 0
  puts "Factorial is not defined for negative numbers."
else
  result = factorial(number)
  puts "The factorial of #{number} is #{result}."
end
```

- Make note of where the backtick button is located. 
- It should appear next to backspace key, but it may vary based on your keyboard layout.

<img src="https://github.com/Lampiranta/github-docs-example/assets/39466981/5db575bc-654b-463f-add1-90d3180db58a" alt="Image Description" width="700px" />

Good cloud engineers use codeblocks for both code and errors that appear in the console.

```bash
An error occurred: divided by 0
Backtrace:
example.rb:2:in `/'
example.rb:2:in `divide'
example.rb:8:in `<main>'
```
>Here is an example of using a codeblock for an error that appears in bash.

## Step 3 - Use Github Flavored Task Lists

Github extends Markdown to have a list where you can chack off items.  [<sup>[1]</sup>](#references)

 - [x] Finish Step 1
 - [ ] Finish Step 2
 - [ ] Finish Step 3 

# Step 4 - Use Emojis (Optional)
GitHub Flavored Markdown (GFM) supports emoji shortcodes.
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: |
| Cloud with lightning | `:cloud_with_lighting:` | :cloud_with_lighting: |

# Step 5 - How to create a table

```md
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: |
| Cloud with lightning | `:cloud_with_lighting:` | :cloud_with_lighting: |
``` 
Github extends the functionality of Markdown tables to provide more alignment and table cell formatting options [<sup>[2]</sup>](#references)


## References
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/) 
- [Basic writing and formatting syntax (Github Flavored Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) 
- [GFM - Task Lists](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists) <sup>[1]</sup>
- [GTM - Emoji CheatSheet](https://github.com/ikatyang/emoji-cheat-sheet/tree/master)
- [GFM Tables ( with extensions)](https://github.github.com/gfm/#tables-extension-) <sup>[2]</sup>
