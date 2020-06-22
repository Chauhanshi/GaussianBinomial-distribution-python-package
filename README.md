# GaussianBinomial-distribution Documentation


## Installation 

> To use this package, follow steps and type in terminal:

>- `pip install matplotlib`
>- `pip install GandB-distributions`

> Once you have install the file in your python environment, you can import this package. Type:

>- `import gandb_distributions`


> For Conda users: 

>- `conda install matplotlib`
>- `conda install pip`
>- `pip install GandB-distributions`

> Once the package is installed 

>- `import gandb_distributions`


This package has two class for now- Gaussian and Binomial. You can create objects using Gaussian() and Binomial()

Object has mean, and standard deviation as attribute. (default mean = 0 and stdev = 1)

Gaussian distribution class for calculating and visualizing a Gaussian distribution.
    
     Attributes:
        mean (float) representing the mean value of the distribution
        stdev (float) representing the standard deviation of the distribution
        data_list (list of floats) a list of floats extracted from the data file

 calculate_mean(self)
 Method to calculate the mean of the data set.
        
calculate_stdev(self, sample=True):

Method to calculate the standard deviation of the data set.
        

read_data_file(self, file_name, sample=True)
    
        Method to read in data from a txt file. The txt file should have
        one number (float) per line. The numbers are stored in the data attribute. 
        After reading in the file, the mean and standard deviation are calculated
   
plot_histogram(self):
        Method to output a histogram of the instance variable data using 
        matplotlib pyplot library. 

plot_histogram_pdf(self, n_spaces = 50):

        Method to plot the normalized histogram of the data and a plot of the 
        probability density function along the same range		
		
		
class Binomial(Distribution):
    Binomial distribution class for calculating and 
    visualizing a Binomial distribution.
    
    Attributes:
        mean (float) representing the mean value of the distribution
        stdev (float) representing the standard deviation of the distribution
        data_list (list of floats) a list of floats to be extracted from the data file
        p (float) representing the probability of an event occurring
        n (int) number of trials


plot_bar_pdf(self):
	 Function to plot the pdf of the binomial distribution		
		

