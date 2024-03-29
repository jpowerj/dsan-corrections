**DSAN 5450: HW1 Corrections / Clarifications**

*(Note: If you are working in **Colab** alone, these updates are automatically applied (at the time given in the timestamps for each bullet point below). This listing is just in case (a) you want to update an answer in light of a correction/clarification, or (b) you are **downloading** the notebook to work offline, in which case you'll need to manually update your local copy)*

* \[*2024-02-09, 8:45pm EST*; Fixed on server side\] The hidden tests for **Questions 4.8.2, 4.8.3, and 4.10.2** were erroneously failing when `y_train`/`y_test` was an $N \times 1$ `DataFrame` rather than a `pd.Series` with length $N$. Since scikit-learn accepts both, the autograder has now been updated to accept both as correct (as long as the size is correct!)
* \[*2024-02-09, 6:30pm EST*; Fixed on server side\] The hidden test for **Question 4.7.1** has been updated to use a lower threshold for the accuracy rate, to handle random variation across runs.
* \[*2024-02-09, 4:30pm EST*; Fixed in Colab versions\] In **Part 4.12**, the required test accuracy threshold has been lowered from 90% to **85%**! So, if you are able to achieve a test accuracy of `0.85` or greater, you are done with this problem!
* \[*2024-02-01, 5:30pm EST*; Fixed in Colab versions\] Questions 3.3a, 3.3b, and 3.3c should have an additional option "Indeterminate". For those working in local copies, you can update the Q3.3a-response cell contents to: `q3_3a_response = "" # @param ["", "True", "False", "Indeterminate"]`, and similarly for Q3.3b-response and Q3.3c-response.
