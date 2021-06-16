# Introduction to Git and GitHub for Social Scientists

Liying Wang, Anwesha Pan, Gayoung Park, Delaney Glass, Ben Marwick

Our workshop slides can be found <a href= https://drive.google.com/file/d/1clOau7UGIq3mhp5-25O18tn3Q0ndqL4k/view?usp=sharing"> here </a>

## Schedule: 

- Welcome and schedule of workshop 
- Motivation for using Git and GitHub: why is this good to use? What is it similar to? 
- Define key tools & concepts such as Git, GitHub, remote, local, commit, push, pull 
    + Activity 1: tour of GitHub page, go to your GitHub account and follow some people, make a repository
- Define fork, clone and pull request 
    + Activity 2: need to work in pairs, learn to fork, commit, and pull requests on GitHub. Using RStudio for cloning, editing, and pushing. Look at commit history and blame view on GitHub 
- Collaborating and resolving merge conflicts 
    + Activity 3: need to work in pairs, learn to collaborate with Git & RStudio. Do the full cycle of fork, clone, commit, identify and resolve merge conflicts
- Summary and conclusion 

## Setup instructions

Before you join the workshop, please make sure you have the most recent versions of Git, R and RStudio installed on your computer. Here's how to get those programs:

  <h3>Git</h3>
  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported
    web browser</a>.
  </p>
  <p>
    You will need an account at <a href="https://github.com/">github.com</a>
    for parts of the Git lesson. Basic GitHub accounts are free. We encourage
    you to create a GitHub account if you don't have one already. Make sure to check your email for a message from GitHub and click the link to confirm your email address with GitHub before joining the workshop. 
    Please consider what personal information you'd like to reveal. For
    example, you may want to review these
    <a href="https://help.github.com/articles/keeping-your-email-address-private/">instructions
    for keeping your email address private</a> provided at GitHub.
  </p>

<h4 id="git-windows">Windows</h4>
<a href="https://www.youtube.com/watch?v=339AEqk9c-8">Video Tutorial</a>
<ol>
<li>Download the Git for Windows <a href="https://git-for-windows.github.io/">installer</a>.</li>
<li>Run the installer and follow the steps below:
<ol>
<li>
                Click on "Next" four times (two times if you've previously
                installed Git).  You don't need to change anything
                in the Information, location, components, and start menu screens.
</li>
<li>
<strong>
                Select “Use the nano editor by default” and click on “Next”.
</strong>
</li>
<li>
                Keep "Use Git from the command line and..." selected and click on "Next".
                If you forgot to do this programs that you need for the workshop will not work properly.
                If this happens rerun the installer and select the appropriate option.
</li>
<li>Click on "Next".</li>
<li>
                Keep "Checkout Windows-style, commit Unix-style line endings" selected and click on "Next".
</li>
<li>
<strong>
                Select "Use Windows' default console window" and click on "Next".
</strong>
            </li>
<li>Click on "Install".</li>
<li>Click on "Finish".</li>
</ol>
</li>
<li>
          If your "HOME" environment variable is not set (or you don't know what this is):
<ol>
<li>Open command prompt (Open Start Menu then type <code>cmd</code> and press [Enter])</li>
<li>
              Type the following line into the command prompt window exactly as shown:
<p><code>setx HOME "%USERPROFILE%"</code></p>
</li>
<li>Press [Enter], you should see <code>SUCCESS: Specified value was saved.</code></li>
<li>Quit command prompt by typing <code>exit</code> then pressing [Enter]</li>
</ol>
</li>
</ol>
<p>This will provide you with both Git and Bash in the Git Bash program.</p>

<h4 id="git-macosx">macOS</h4>
<p>
        Please open the Terminal app, type <code>git --version</code> and press
        <kbd>Enter</kbd>/<kbd>Return</kbd>. If it's not installed already,
        follow the instructions to <code>Install</code> the "command line
        developer tools". <strong>Don't click</strong> "Get Xcode", because that will
        take too long and is not necessary for our Git lesson.
        After installing these tools, there won't be anything in your <code>/Applications</code>
        folder, as they and Git are command line programs.
        <strong>For older versions of OS X (10.5-10.8)</strong> use the
        most recent available installer labelled "snow-leopard"
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
        Because this installer is not signed by the developer, you may have to
        right click (control click) on the .pkg file, click Open, and click
        Open in the pop-up dialog. You can watch
        <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">a video tutorial about this case</a>.
</p>

<h4 id="git-linux">Linux</h4>
<p>
        If Git is not already available on your machine you can try to
        install it via your distro's package manager. For Debian/Ubuntu run
        <code>sudo apt-get install git</code> and for Fedora run
        <code>sudo dnf install git</code>.
</p>


<h3>R & RStudio</h3>

<p>
    <a href="https://www.r-project.org">R</a> is a programming language
    that is especially powerful for data exploration, visualization, and
    statistical analysis. To interact with R, we use
    <a href="https://www.rstudio.com/">RStudio</a>.
</p>


<h4 id="r-windows">Windows</h4>
<a href="https://www.youtube.com/watch?v=q0PjTAylwoU">Video Tutorial</a>
<p>
        Install R by downloading and running
        <a href="https://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
        from <a href="https://cran.r-project.org/index.html">CRAN</a>.
        Also, please install the
        <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
        Note that if you have separate user and admin accounts, you should run the
        installers as administrator (right-click on .exe file and select "Run as
        administrator" instead of double-clicking). Otherwise problems may occur later,
        for example when installing R packages.
</p>

<h4 id="r-macosx">macOS</h4>
<a href="https://www.youtube.com/watch?v=5-ly3kyxwEg">Video Tutorial</a>
<p>
        Install R by downloading and running
        <a href="https://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
        from <a href="https://cran.r-project.org/index.html">CRAN</a>.
        Also, please install the
        <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
</p>

<h4 id="r-linux">Linux</h4>
<p>
        You can download the binary files for your distribution
        from <a href="https://cran.r-project.org/index.html">CRAN</a>. Or
        you can use your package manager (e.g. for Debian/Ubuntu
        run <code>sudo apt-get install r-base</code> and for Fedora run
        <code>sudo dnf install R</code>).  Also, please install the
        <a href="https://www.rstudio.com/products/rstudio/download/#download">RStudio IDE</a>.
</p>

## Join Zoom Meeting

You can join our workshop at this link:
https://washington.zoom.us/j/97631523248?pwd=eGtsNG1MMTJkTzVnQy9YK3lLYjFyQT09

Time: Aug 26, 2020 09:00 AM Pacific Time (US and Canada)

Meeting ID: 976 3152 3248

Passcode: 549527

Content on this site is licensed under a [Creative Commons Attribution 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/).
