
# M2installNLP

**Temporary Note**: In the below documentation, all CODES have been written in a monospace font for better clarity.

## Install Miniconda

1. Download Miniconda from the following link: 
   [Miniconda for MacOSX-arm64](https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.pkg)
   
   - Follow the standard installation process for Apple products. Simply double-click the downloaded `.pkg` file or single-click it from your browser.

## Activate Miniconda

2. Open your terminal and input the following command:

conda activate /Users/<YOUR_USERNAME>/miniconda3


Replace `<YOUR_USERNAME>` with your actual username. For example:

conda activate /Users/simonbian/miniconda3


3. If the above step doesn't work, execute the following command to see a list of environments:

conda env list


Identify the path that contains "miniconda" or its variants, then activate it:

conda activate /YOUR_IDENTIFIED_PATH

For instance:

conda activate /Users/simonbian/miniconda3


## Install Packages

4. Save the attachment I sent in this email to your Desktop. Navigate to your Desktop in the terminal with:

cd ~
cd Desktop


5. Once `requirements.txt` is on your desktop, execute the following command to install the required packages:

cat requirements.txt | xargs -n 1 pip3 install


Note: Any output in red is expected, as it's machine dependent.

6. Finally, install the necessary TensorFlow packages:

pip3 install tensorflow-macos
pip3 install tensorflow-metal


After this, you can delete `requirements.txt` if desired.

## Execution

7. You can now execute the software as usual.

**Note**: Throughout this guide, `pip3` and `pip` are interchangeable, as are `miniconda` and `miniconda3`.


# New Steps if you are failing the Senti analysis (may not succeed - in beta testing still)


## 8. Install Homebrew
Homebrew is a free tool that helps you install software onto your computer. Think of it as an app store for your command line!

Open Terminal: This can be found in your Applications folder, inside the Utilities folder. It's a program that allows you to interact with your computer using text commands.
Install Homebrew: Once you have Terminal open, copy the line of code below and paste it into Terminal, then press Enter.
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Follow any prompts that appear. This process will install Homebrew onto your computer. It might ask for your computer's password, which is normal. Just type in your password and press Enter.

## 9. Download the Brewfile
The Brewfile is a list of software that we'll be using for our course. It tells Homebrew exactly what to install.


Go to the provided GitHub page.


Find the Brewfile I've uploaded and download it. Make sure you remember where you've saved it on your computer, such as the Downloads folder.


## 10. Install the Dependencies
Now that you have the Brewfile, we'll use it to install the software we need.


Open Terminal again (if you closed it).

** Navigate to the Directory with the Brewfile : If you saved the Brewfile in your Downloads folder, you'd type the following command into Terminal and then press Enter:
```
cd ~/Downloads
```
Install the Software: Now, type the following command into Terminal and press Enter:
```
brew bundle install
```

