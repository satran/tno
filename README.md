# tno

`tno` is a way to organize your life using text files. `tno` stands for Text Not Org. The idea came from using Orgmode. The problem with Orgmode was that it was very tightly coupled with Emacs. Even though an Orgmode file was just a text file it was difficult to integrate it with other tools. When I tried to open an Orgmode file in another text editor it was filled with formatting data and the I could not see the actual content. TNO was thus created as I wanted to use something like Orgmode. 

## Tasks
TNO was primarily created for tasks. Tasks are lines that start with a `* [ ]`. Here is an example task:

    * [ ] this is a task
    
A task can be of different stages. The most common stages are:
- open, represented by [ ]
- done is represented by [x]

This is the basics of tasks. More information can be found in its [specification](tasks.md).