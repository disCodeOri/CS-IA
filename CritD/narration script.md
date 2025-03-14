This video demonstrates the functionality and extensibility of the Information Management System, a web application designed to streamline academic workflows for my client, addressing the inefficiencies of his paper-based system.

The application begins with secure user authentication, powered by Clerk. Users can easily sign-in or sign-up to access their personalized workspace, and any unauthorised user will be redirected to the log in page, ensuring data privacy and security as per success criterion 17.

Upon login, users are presented with a clean and intuitive dashboard, fulfilling success criterion 15 for a user-friendly interface. The sidebar provides easy navigation to the core components, while the workstage area offers a central mission control for information management with multiple different views to accomodate the user's unique workflow.

Let's explore the Cookie Jar component first. This component was requested by the client to cater to their motivational needs, allowing him to create and manage digital 'cookies', which are visual representations of their achievements, positive affirmations, or quotes for self-motivation.

As you can see, creating a new cookie is fairly straightforward. Users can define a name and description and the Cookies are persistently saved using Firebase Firestore, ensuring data is available across sessions. Additionally, the implementation for editing and deleting cookies is also intuitive. Furthermore, the drag-and-drop functionality has been implemented using the `@dnd-kit` library, enabling users to reorder cookies to personalize their motivational space, meeting success criteria 1, 2, 3, 4, 5 and 9.

Next, we have the Doubt Tracker component, designed to help users log, manage, and resolve academic doubts.

Users can easily create new doubt entries with titles and descriptions. The DoubtTracker component supports status management where doubts can be marked as 'Resolved' by providng a solution into the solution textbox. Any resolved Doubt can be reopened and the action of reopening removes the previously stored solution. Addressing success criteria 4, 8 and 10.

The voting and commenting functionalities have also been implemented to allow the user to organise their list of doubts, and store any additional information such as explanations and any nuances to consider. The user can also reply to any comment and this enables creative freedom in storing additional information.

This component was designed to largely mimic the UI of reddit.com, which was identified as a site where my client was most actively engaged with. Implementing a familiar UI contributes to the user's request to have a "plug and play" experience. Meeting success criteria 6, 7, 15 and 19.

Next Up, The CuriositySpace, or Idea Tracker component, mirrors the DoubtTracker component in functionality, but focuses on capturing and developing creative ideas outside of a strictly academic environment that is the DoubtTracker component.

The User can similarly create, resolve, vote, and comment on ideas, providing a dedicated space for brainstorming and idea management, fulfilling success criterion 11.

Additionally, it is to be clarified that both the CuriositySpace component and the DoubtTracker component are user specific and do not have collaborative access between multiple users.

The To-Do List component offers a flexible and visual way to manage tasks.

It allows users to organize tasks into sections and columns, reflecting the client's preferred multi-list workflow. Within the columns, the users can create tasks and also add subtasks for detailed breakdowns and additionally, track completion by checking or unchecking the tasks. Furthermore, a drag-and-drop functionality between and within columns allows for easy task reorganization, fulfilling success criteria 5 and 12.

For comprehensive note-taking, the Notebooks component provides a hierarchical notebook system, attempting to mimic the multi-sheet workflow of my client.
And in the landing page of the component users can create, preview, open, and delete notebooks. Within the notebooks the users can create/edit/delete sections, columns, and notes, closely mirroring the physical notebook format of my client with flexible hierarchical organization. Notes within notebooks can be reordered using drag-and-drop, effectively digitizing and enhancing the client's paper-based notebook system, and thus meeting success criteria 5, 13, and 15.

Finally, the Stage Manager component addresses the client's need for a 'mission control' workspace.

Users can create multiple Spaces, each containing Windows that can represent different information streams. Windows can be edited, moved, resized, and their layouts and contents are persistently saved across sessions, directly addressing the client's desire for a digital equivalent of their multi-sheet paper layout for specific moments, fulfilling success criterion 14.

Throughout the application, data is synchronized in real-time across devices using Firebase Firestore, ensuring seamless access from anywhere, as demonstrated here by the instantaneous changes reflecting across two instances of the application, fulfilling success criterion 18.

The application is also designed to accomodate for cross-browser compatibility, functioning correctly on major browsers like Chrome, Firefox, Safari, and Edge.

To ensure maintainability and extensibility, the application is built using a component-based architecture with React and NextJS14, leveraging TypeScript for enhanced code quality. The codebase is thoroughly commented, allowing for easy maintenance and future development by third parties. Which finally addresses the success criterion 20.

In conclusion, the Information Management System successfully addresses the client's needs for a convenient, efficient, and user-friendly tool to manage academic and personal information, and subsequently meeting all defined success criteria. For future development, developer recommendations include expanding user accessibility and adding study hour tracking features, as detailed in Criterion E.
