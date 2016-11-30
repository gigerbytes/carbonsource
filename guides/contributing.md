##Contributing
All of the code submitted to carbonsource should adhere to the styles outlined in this guide.
In order to keep iteration fast and code throughput high, we will be using github, and a certain branch flow, to allow for frequent testing and code review without slowing down development.


The branches will be laid out something like this:

###Branch structure

                        |- Feature
Master <- Development <-|- Release
                        |- Hotfix

###Branch definitions:
- Master: Main production code goes here. This will be the code that is currently running on the website.
- Development: The latest test build with a new feature implemented. Extra QA/ unit + feature testing should happen here.
- Feature branches: Branches off from development. Usually stored locally on developer machines, although collaboration also happens.
  - Branch off from: Development
  - Merge into: Development
  - Branch naming convention: anything except the other branch names.
- Release branches: These branches support a build as the final bug fixing and build preparation happen. These branches exist so that the development branch can become free for the next set of features to start rolling in.
  - Branch off from: Development
  - Merge into: Development or Master.
  - Branch naming convention: \"release-\*\"
- Hotfix branches:
  - Branch off from: Master
  - Merge into: Development and Master
  - Branch naming convention: \"hotfix-\*\"

###Pull request structure:
Pull requests are a great time for additional code review, and general improvement of features.
For this reason, we  require all code contributions to follow this pattern:
  - 1. Find an open issue with a "Ready" tag, and create a new branch off of development named after the issue.
  - 2. Write tests. As much as possible, try to write tests for your code! Test driving is ideal, but not required, however at least a reasonable attempt at unit/ feature testing should be made. Good testing habits (see testing in rails below) can improve the quality of code tremendously, and even the final product
  - 3. Write code! Look through the rest of our codebase, go on stackoverflow or check out some of the other material here in the guides section! There is lots to look at for inspiration and many people to turn to for help.
  - 4. Commit frequently, to create a log of the changes you implement.
  - 5. Once you deem the issue to be nearing completion, open a pull request to the development branch, and get ready for some more work!
  - 6. Read all of the comments people make, and implement any reasonable suggestions or improvements. Other people can definitely contribute code at this stage! In fact, collaboration at this stage increases productivity tremendously.
  - 7. Once all of the commenters are happy, someone will merge the request into development. At this point, your code will undergo additional testing in the development branch, and other features will be merged in with it. Once we reach a certain point, a new release branch is created, which undergoes more rigorous end user and interface testing. Final patches are applied, and the code is shipped on to Master. 

###Testing:
- https://robots.thoughtbot.com/how-we-test-rails-applications
