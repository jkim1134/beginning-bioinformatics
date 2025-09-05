# AI Use Log
- Tool/model & version:
- What I asked for:
- Snippet of prompt(s):
- What I changed before committing:
- How I verified correctness (tests, sample data)


9/4/25
-ChatGPT-4
-explain how to sort odd integers from a numerical range from 5 to 27
-![Uploading image.png…]()
Use Python's range() function to create numbers from 5 to 27:
range(5, 28)  # 28 because the stop value is exclusive
Use a list comprehension to get only numbers where num % 2 == 1:
odd_numbers = [num for num in range(5, 28) if num % 2 == 1]
-tested for accuracy by comparing to sample question and answer

9/5/25
-ChatGPT-4
-explain enumerate in python
-enumerate() is a built-in Python function that lets you loop over a sequence (like a list, tuple, or string) and get both:
The index (position)
The element (value)
-applied "for line_num, line in enumerate(f, start=1):" 
-tested validity by attaching and running with command 
