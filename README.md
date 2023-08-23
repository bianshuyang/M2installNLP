# M2installNLP
Temporary

In the below documentation, all CODES have been written in another font for better clarity.
Install miniconda by: https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.pkg As always like other Apple product, double click / single click from browser, since they are M2 users.
Once done, navigate to terminal and input the following code, where the bold line should be the user's name
conda activate /Users/USERNAMETOBEREPLACED/miniconda3
For example, mine is /Users/simonbian/miniconda3. If this step fails, users will have to first execute conda env list to visualize what "miniconda" is called on their machine, like following:

Once they identify where miniconda or analogs of "miniconda" is, they copy the highlighted file, and execute 
conda activate /THATCOPIEDDIRECTORYINBLUE
For instance, conda activate /Users/simonbian/miniconda3
Save the attachment I sent in this email in Desktop. Then use the following command to ensure one is at Desktop:
cd --
cd Desktop
Once requirements.txt is in their desktop, in the same terminal, type the following code and execute
cat requirements.txt | xargs -n 1 pip3 install
Let the user know that anything red is expected, since it is machine dependent.
Finally, execute the following:
pip3 install tensorflow-macos
pip3 install tensorflow-metal
  Then they will be free to delete "requirements.txt" when they want. Step 3 can be done in any way so long as the user can finally navigate to a folder with requirements.txt, the only purpose is to quickly install all the packages that are native to M2.
Then they can execute the software as usual. Pip3 and pip shall be interchangeable words, as is miniconda with miniconda3.
