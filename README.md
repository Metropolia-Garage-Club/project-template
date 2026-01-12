# Metropolia Garage Project Template
## Repository for materials related to Metropolia Garage projects

## Please take the time to read this MD carefully! It contains all instructions on how to provide your project to us!

This is a repository created to serve as a standard template for all official Metropolia Garage projects. 
In this repository, you can find the standard project folder structure, project documentation template and guide as well as introduction to how to use git and github.

### REPLACE THIS MD WITH DEPLOYMENT INSTRUCTIONS!

Your deployment instructions must include image of a program flowchart!

Your deployment instructions must be comprehensive enough for someone unfamiliar with your work to get it running!

### Required work for course credits

If you are doing project work for AIoT / Robo -garages as part of a course, there are few requirements that **you must fulfill**:

#### Documentation requirements

We expect you to not only properly document your project, but also to write usage instructions. Replace THIS FILE with the deployment instructions. Markdown is a great way to easily format and visualize usage and deployment instructions for your project on the repository front page. 
If you are new to Markdown, refer to this [cheatsheet](https://github.com/adam-p/markdown-here/wiki/markdown-cheatsheet).

For the actual project documentation, there is a formatted template in the Docs folder you can use if you want, but you don't need to use it. The important thing is that the format and language of the documentation follows the Metropolia Thesis guidelines. 

*If you are doing your Innovation project report / Thesis, that will act as your project report for the PROJECT! In that case, please upload it with the project files or link to it in theseus OR provide a garage employee with the files on TEAMS!*

The report should include atleast the following:

- What was the project about?
- What are the things you did?
- What choices did you make with your implementation and why? (Eg. choices between different software / libraries)
- What were the problems you faced and how did you solve them?
- What work remains to be done or what issues need to be fixed?


And finally, list the tools/software you used for the project and provide brief description of what each of them are for. 

In general, the project report should be technical in nature. Focus on writing about the technical implementations. This will be important for the garage as well as the companies, which might want to implement your project into their systems. Describe all the systems and sub-systems of your work in clear manner. Creating a program flowchart is also very appreciated!

You are the expert of your own project and it is critical that the work and innovation you have spent your time on is easily available to us in the future! 


### How to proceed
If you don't have Git installed yet, refer to [setting up Git](https://docs.github.com/en/get-started/git-basics/set-up-git).

We highly recommend you to start with the amazing [First Contributions](https://github.com/firstcontributions/first-contributions) guide if you are new to GitHub. 

This template is made with forking and pull requests in mind to systemize workflow and make it easy for Metropolia Staff to access your project later, while allowing you to work as freely as possible

### Project structure

In this project template, you can find a readymade folder structure. Your project may not need some of the folders. **DELETE THE FOLDERS YOU DON'T NEED!.** 
**Otherwise, please use the provided structure.**

#### Overview of the folders

##### Deployment
* Any files or general dependencies that are necessary to get the project running

##### Docs
* **Project Report**, Notes, Guides, you can find the Word Documentation Template here with basic structure and formatting. Otherwise, use Metropolia Thesis structure. 

##### Firmware
* Files and software, which are necessary to get your hardware running

##### Hardware
* Schematics, parts and other things related to your project hardware

##### Media
*  All media material related to the project, sorted

##### Presentation
*  Your power point presentations or posters if you have any

##### References
*  Scientific papers, datasheets, web links, research material - Please name them in a clear manner

##### Software
*  Your actual code, ML models, libraries etc.

#### Example project structure

1.  Project-Name/   

 2. │   

 3. ├──  docs/            # Documentation and reports   

 4. │   ├── project-report.docx   # Main project report   

 5. │   ├── requirements.txt  	# Project requirements & specs     

 9. │      

11. ├──  software/    # AI, IoT, and application code
24. │   ├──  deployment/ # Deployment files, Docker, cloud configurations   

25. │   │   ├── docker/   

26. │   │   ├── k8s/   

27. │   │   ├── cloud-setup/       

14. │   ├── models/      # AI/ML models and training scripts   

15. │   ├── code/     # Project source code, helper scripts, automation   

16. │   ├── tests/       # Unit tests, integration tests   

17. │   ├── README.md    # Explanation of software structure   

18. │   │   

19. │   ├──  firmware/  # Microcontroller firmware (if any)   

20. │   │   ├── esp32/   

21. │   │   ├── jetson/   

22. │   │   ├── raspberry-pi/   

28. │   

29. ├──  hardware/      # Any hardware-related files   

30. │   ├── schematics/      # Circuit diagrams, PCB designs   

31. │   ├── parts-list.xlsx    # List of components and BOM   

32. │   ├── assembly-guide.md  # Instructions for assembling hardware   

33. │   

34. ├──  media/        # Images, videos, marketing materials   

35. │   ├──  photos/         # Pictures of the project   

36. │   ├──  videos/         # Any demo or tutorial videos   

37. │   ├──  graphics/       # Logos, banners, presentation materials   

38. │   

39. ├──  presentations/       # Slides, posters, marketing materials   

40. │   ├── presentation.pptx   

41. │   ├── poster.pdf   

42. │   

43. ├──  references/          # Papers, useful links, background materials   

44. │   ├── papers/   

45. │   ├── links.md   

46. │   

47. ├── .gitignore              # Ignore unnecessary files for version control   

48. ├── README.md               # General project overview   

49. └── LICENSE                 # Open-source license, if applicable  

50.   


### Using Git

#### Getting started

**Clone the repository**: Set it up locally using the command line:
>git clone [repository-URL]

(Downloads a copy of your fork to your local machine)

>cd [repository-name]          

(Moves into the project directory)

**Create your working branch**:
>git checkout -b [your-name]/dev

(Creates and switches to your personal development branch. Use a consistent naming convention, e.g., name/dev)

>git push -u origin [your-name]/dev

(Pushes your branch to the remote repository and sets it as the default upstream for future pushes)

#### Development Workflow

**Create feature branches** off your development branch for specific tasks:
>git checkout -b [your-name]/feature-name

(Creates a new branch for a specific feature, branching from your current location)

**Make your changes** and commit regularly with clear messages:
>git add .

(Stages all modified files for commit)

>git commit -m "Implement feature X"

(Records changes with a descriptive message)

**Merge completed features** back to your development branch:
>git checkout [your-name]/dev

(Switches back to your development branch)

>git merge [your-name]/feature-name

(Integrate your completed feature)

>git push origin [your-name]/dev

(Push the updated development branch to the remote)

Generally, keep your personal development branch as a functional checkpoint and use separate feature branches for work-in-progress. This way you always have a stable version to fall back to.

#### Submitting your work
When your work is ready for final submission, create a pull request to merge into main:

Push your latest changes to your development branch
Go to the repository on GitHub
Click "Pull requests" > "New pull request"
Set base to main and compare to [your-name]/dev
Click "Create pull request"
Add a title and description explaining your changes

We will review your pull request and merge it into the main branch when accepted.
