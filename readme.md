# Bash Scripting  Practical Assignment

**Topic:** Pipes, Redirection, `grep`, `sort`, `uniq`, and `cut`  
**Total Marks:** 30 | **Total Questions:** 10 | **Marks per Question:** 3

---

# Q1. Output Redirection
echo -e "Amit\nRahul\nPriya\nSimran\nKaran" > students.txt
cat students.txt

# Q2. Append Redirection
echo -e "Neha\nVikram\nAnjali" >> students.txt
cat students.txt

# Q3. Using Pipes
cat students.txt | sort

# Q4. Search Text
echo -e "Rohan\nMeera\nKabir\nSonia\nDeepak\nNitin\nPooja\nArjun\nKavita\nManish" > employees.txt
grep "a" employees.txt

# Q5. Case-Insensitive Search
echo -e "Linux is an open-source operating system.\nMany servers run on LINUX distributions.\nLearning linux commands is essential.\nWindows and macOS are different platforms." > notes.txt
grep -i "linux" notes.txt

# Q6. Sorting Data
echo -e "78\n45\n92\n100\n64\n88\n51\n39\n81\n73" > marks.txt
sort -n marks.txt

# Q7. Remove Duplicate Lines
echo -e "Ludhiana\nMohali\nChandigarh\nLudhiana\nDelhi\nMohali\nAmritsar\nLudhiana\nDelhi" > cities.txt
sort cities.txt | uniq

# Q8. Count Duplicate Lines
sort cities.txt | uniq -c

# Q9. Extract Columns
echo -e "ID,Name,Course,City\n101,Amit,React,Mohali\n102,Rahul,Python,Chandigarh\n103,Priya,Flutter,Ludhiana\n104,Simran,Java,Mohali\n105,Karan,DevOps,Delhi" > students.csv
cut -d',' -f2 students.csv

# Q10. Extract Multiple Fields
cut -d',' -f2,4 students.csv