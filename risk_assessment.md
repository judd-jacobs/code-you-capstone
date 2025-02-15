### **Potential Challenges & Solutions**  

### **1. Getting Data from APIs & Files**  

**Possible Problem:**  

- The movie data from TMDb or OMDb might be incomplete or unavailable.  
- Some Oscar-winning movies may not have full details, like missing box office earnings.  

**Solution:**

✅ Try using multiple sources (CSV files or Wikipedia data) to fill in missing details.  
✅ Save API data to a file so you don’t need to keep requesting it repeatedly (this helps avoid API limits).  
✅ If a request fails, wait a few seconds and try again.  

---

### **2. Cleaning Up the Data**  

**Possible Problem:**  

- Some movie titles might be written differently in different datasets.  
- Some values (like box office revenue) might be missing.  
- Acceptance speech text might contain unnecessary words.  

**Solution:**

✅ Remove extra spaces and standardize movie titles so they match across datasets.  
✅ Fill missing numbers with a reasonable guess (e.g., if a runtime is missing, use the average runtime of other movies).  
✅ Use **Python’s NLTK library** to clean the speech text by removing common words like "the" and "a" so only important words remain.  

---

### **3. Writing SQL Queries & Understanding the Data**  

**Possible Problem:**  

- SQL queries might not return the expected results.  
- It might be hard to figure out how to organize the data for easy analysis.  

**Solution:**

✅ Start by **writing simple SQL queries** to check what the data looks like before running complicated queries.  
✅ If a query gives unexpected results, check if the table names and column names are correct.  
✅ Use **LIMIT 10** in your SQL queries to only look at the first 10 rows before working with larger datasets.  

---

### **4. Managing Time & Staying on Track**  

**Possible Problem:**  

- The project might take longer than expected.  
- You might want to add too many features and run out of time.  

**Solution:**

✅ Follow a weekly **plan** to make sure you're working on the most important parts first.  
✅ Avoid adding new features after the first month so you have time to finish what’s already planned.  
✅ Use a **to-do list** or a simple GitHub issue tracker to stay focused.  

---

### **5. Creating Clear Visualizations**  

**Possible Problem:**  

- Graphs might be hard to understand or look confusing.  
- It might be difficult to decide what kind of visualization to use.  

**Solution:**

✅ Use **bar charts** to compare the number of Oscar wins for different genres.  
✅ Use **scatter plots** to check if higher box office revenue leads to more Oscar wins.  
✅ Add **titles, labels, and legends** to every graph so others can understand what they show.  

---

### **6. Preparing the Final Project for Submission**  

**Possible Problem:**
  
- Code might not run correctly on another computer.  
- Some files might be missing when submitting the project.  

**Solution:**

✅ Before submitting, run all the notebook cells in order to make sure everything works.  
✅ Write clear **instructions in the README file** so anyone can follow along.  
✅ List all required Python libraries in a **requirements.txt** file so others can install them easily.
