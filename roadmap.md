

Here's a creative, structured **21-day regex mastery plan** with cheat sheets, examples, tests, and hands-on projects:

---

### **Phase 1: Foundations (Days 1-5)**
**Goal:** Understand core concepts and basic syntax.

**Day 1: Literals & Metacharacters**
- Learn: `.` (any char), `\` (escape), `^` (start), `$` (end)
- Example: Match "cat" vs. `c.t` (matches "cat", "cot")
- Cheat Sheet: [Basic Syntax Table](https://regexr.com/cheatsheet)
- Test: Write regex to match "hello" at the start of a line.

**Day 2: Character Classes**
- Learn: `[abc]`, `[^abc]`, ranges (`[a-z]`), `\d`, `\w`, `\s`
- Example: `gr[ae]y` matches "gray" or "grey"
- Creative Exercise: Create a regex for hexadecimal colors (`#a1b2c3`)

**Day 3: Quantifiers**
- Learn: `*`, `+`, `?`, `{n,m}`
- Example: `\d{2}-\d{2}-\d{4}` for dates like "01-01-2023"
- Test: Match strings with 3-5 vowels in a row.

**Day 4: Anchors & Boundaries**
- Learn: `^`, `$`, `\b` (word boundary)
- Example: `^\d+$` matches strings that are purely numbers
- Game: Regex Crossword ([regexcrossword.com](https://regexcrossword.com))

**Day 5: Grouping & Alternation**
- Learn: `()`, `|`, backreferences `\1`
- Example: `(cat|dog) food` matches "cat food" or "dog food"
- Project: Extract phone numbers in multiple formats.

---

### **Phase 2: Intermediate (Days 6-10)**
**Goal:** Master advanced patterns and efficiency.

**Day 6: Lookarounds**
- Learn: `(?=...)` (lookahead), `(?<=...)` (lookbehind)
- Example: `foo(?=bar)` matches "foo" only before "bar"
- Test: Match "apple" not followed by "pie".

**Day 7: Flags & Modes**
- Learn: `i` (case-insensitive), `g` (global), `m` (multiline)
- Example: `/apple/ig` matches "Apple", "APPLE", etc.
- Creative Task: Write a case-insensitive regex for valid emails.

**Day 8: Escaping & Special Cases**
- Learn: Escaping metacharacters (`\.`), `[\b]` (backspace)
- Example: Match a literal "$" with `\$`
- Quiz: Fix this invalid regex: `*test*`

**Day 9: Unicode & POSIX**
- Learn: `\p{L}` (Unicode letters), `[[:digit:]]`
- Example: `\p{Sc}` matches currency symbols ($, €, etc.)
- Exercise: Match emojis using Unicode properties.

**Day 10: Performance Optimization**
- Learn: Avoid `.*` greediness, use atomic groups `(?>...)`
- Example: Optimize `a.*b` → `a[^b]*b`
- Debugging: Use [Regex101](https://regex101.com) to analyze steps.

---

### **Phase 3: Advanced (Days 11-15)**
**Goal:** Tackle complex scenarios and edge cases.

**Day 11: Backreferences & Substitutions**
- Learn: `\1`, `\k<name>`, replacement patterns
- Example: Swap first/last name: `(\w+) (\w+)` → `$2, $1`
- Project: Reformat dates from MM/DD/YYYY to YYYY-MM-DD.

**Day 12: Conditional Patterns**
- Learn: `(?(?=condition)true|false)`
- Example: `(?(?=\d{3})\d{3}-|\d{2}-)\d{2}-\d{4}`
- Test: Match 5-digit or 9-digit ZIP codes conditionally.

**Day 13: Recursive Patterns**
- Learn: `(?R)`, subroutine calls
- Example: Match nested parentheses `(\((?:[^()]++|(?R))*\))`
- Challenge: Validate mathematical expressions.

**Day 14: Possessive Quantifiers & Atomic Groups**
- Learn: `*+`, `++`, `(?>...)`
- Example: `a++b` fails faster than `a+b` in some cases
- Exercise: Compare performance of `.*?` vs. `[^"]*`.

**Day 15: Real-World Applications**
- Learn: Data validation (emails, URLs), log parsing
- Example: Extract IP addresses from logs: `\b\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\b`
- Project: Build a password strength checker with regex.

---

### **Phase 4: Mastery (Days 16-21)**
**Goal:** Solidify skills through practice and creativity.

**Day 16: Regex Golf**
- Play: [Regex Golf](https://alf.nu/RegexGolf) to sharpen pattern recognition.

**Day 17: Code Integration**
- Learn: Regex in Python, JavaScript, or your preferred language.
- Example: Python's `re.findall(r'\b\w{5}\b', text)`.

**Day 18: Debugging & Visualization**
- Use: [Debuggex](https://www.debuggex.com) to visualize regex flow.

**Day 19: Security Considerations**
- Learn: Avoid catastrophic backtracking (e.g., `(x+)+y`).

**Day 20: Final Project**
- Build: A regex-based tool (e.g., markdown parser, data scrubber).

**Day 21: Teach Someone Else**
- Create: A 5-minute lightning talk or cheatsheet for peers.

---

### **Resources**
1. **Cheat Sheets:** 
   - [Regex Cheat Sheet](https://www.rexegg.com/regex-quickstart.html) 
   - [Cheatography](https://cheatography.com/davechild/cheat-sheets/regular-expressions/)
2. **Interactive Tools:** 
   - [Regex101](https://regex101.com) 
   - [RegExr](https://regexr.com)
3. **Books:** 
   - *Mastering Regular Expressions* by Jeffrey E.F. Friedl

---

**Key Tips:**
- Start simple, then layer complexity.
- Use `.*` sparingly; prefer explicit patterns.
- Test on real data to catch edge cases.

Let me know if you want me to dive deeper into any concept! 🚀
