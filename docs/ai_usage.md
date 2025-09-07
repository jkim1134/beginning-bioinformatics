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


9/6/25










-ChatGPT-4
-Explain the following code from Bio.SeqIO import parse def gc_content(seq): gc = seq.count('G') + seq.count('C') return (gc / len(seq)) * 100 max_gc_id = "" max_gc_value = 0 for seq_record in parse("rosalind_gc (1).txt", "fasta"): gc = gc_content(seq_record.seq) if gc > max_gc_value: max_gc_value = gc max_gc_id = seq_record.id print(max_gc_id) print(f"{max_gc_value:.6f}")
-To find the FASTA sequence in a file that has the highest GC-content percentage and print:
its ID
its GC content to 6 decimal places
-gc_content()	Calculates % of G and C bases in a sequence
parse(..., "fasta")	Reads sequences one by one from the FASTA file
max_gc_value	Tracks the highest GC percentage
max_gc_id	Tracks which sequence had that highest GC content
print()	Outputs final result
-Tested for corectness by bunning code in rosalind
