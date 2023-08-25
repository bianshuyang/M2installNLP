
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


Steps to Set Up Your Development Environment
(The steps below start from 8 as you've mentioned there are already 7 steps ahead)

<font color="red">
8. Install Homebrew

Ensure you have Homebrew installed. If you haven't, follow the instructions below:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

9. Download the Brewfile

Navigate to the provided GitHub page and download the Brewfile I've uploaded.

10. Install the Dependencies

Once you have the Brewfile, open your terminal, navigate to the directory where you downloaded the Brewfile, and run:

```bash
brew bundle install
```
</font>
