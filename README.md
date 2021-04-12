**Check out my reports here:**
https://cameron-it.github.io/Triathlon/

# Triathlon
Analyses of my triathlon data. I have been a triathlete since 2018, but my training became a lot more serious in 2019 when I realized how much I enjoyed endurance sports. Each year, I will produce a report that goes over my training for that year. I will then use the data to decide where I have been doing well in training and to identify areas of improvement. If you think I should do additional analyses, please reach out to me. I would be happy to go exploring through the plethora of data I have captured (about 500 entries a year).

*Data collection* 
I compile all my training data in commonly used software for athletes, called Training Peaks. Training Peaks takes my data recorded on my devices (Forerunner 945 watch, Garmin Edge 530, Garmin HR-Tri, Garmin HR-Duo, Wahoo Kickr Core, and Assiomo Duo) and stores it within individual files for each workout. Heart rate is recorded as the number of beats per minute, power is recorded in watts, cadence is recorded in steps per minute, and velocity is recorded in meters per second. The data is downloaded from training peaks as a single .csv file for each training season. It is this .csv file that I use for analysis and visualization.

*Analysis and visualizations* 
My reports are produced using R notebooks and published as html files. Therefore, I use a bit of html code for formatting and the data is processed, analyzed, and visualized using R. I chose notebooks because I can create reproducible reports using the same template every year. It also helps you follow along by showing the code chunks that produce the summary data, visuals, and charts I have created. It's quite transparent! That is the way I like it.

*Website generation* 
I use the R markdown render_site() function to generate a directory (docs) containing all the necessary files for turning my notebooks into a single website. All the subdirectories and files in docs are automatically generated when I render the site. One downside to this function is that all the files I need to render a website must be in the root directory ("Triathlon"" in this case), so that is why you see my .Rmd and .yml files floating around among the other directories in this repository. The _site.yml file is used to configure the website content/features and push the results to the docs directory. The docs directory is explicitly named that because GitHub Pages can only render a site from either the main branch or a docs directory within the main branch. This limitations is worth it because it is a matter of clicking two buttons to generate a website from your repository using GitHub Pages.
