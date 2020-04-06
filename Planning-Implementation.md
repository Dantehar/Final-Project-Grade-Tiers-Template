## Model, View, Controller

### The Model
#### Setup the Model 
* Represents data to be displayed, manipulated, and retrieved
* Comprises one or more classes (or objects) that separate data into logical groups
* Represents knowledge and expertise related to a specific problem domain
* Defined to match the real-world objects they represent

#### Model Objects
* Properties hold the encapsulated data of the object
* Methods (or functions) and computed properties provide the logic to manipulate the properties or perform actions on the object
* Initializers set up your objects before they are used for the first time

As you've learned, a model refers to the data your app will capture and/or display. Model objects are specific types of data. A very simple app may have one model type, but even trivial applications may have many related model types.
To begin your project plan, review every feature on your list, then consider all the information you'll need and how you might group it. 

✏️ Answer the following questions:
1. What are the primary types of data that the app will work with?
2. What data will the user input into the app?
3. What data will your app display?
4. Where will the app get the data?
5. What APIs or frameworks will the app access?
6. How does the data relate to other data?
7. How will you persist, or save, the data?

* If you have two types of related data, consider their relationship. _How can you access all the data you need from the data you already have?_ For example, if you were to build a simple shopping app, you may want to view the order history of a particular customer.If you have an instance of an Order object, you should have a property that points to the Customer. But if you have an instance of a Customer, you may have a property that points to an array of Order instances.

✏️ Write down each model type you'll need to define, along with a list of corresponding properties. Add to your list any helper methods you may need for persistence as well as any querying relationships.


### The View
* List the different views or scenes your app will display
* Determine which views or scenes you can reuse 
* Determine the types of views that you can use to display the data:  
  * Table view 
  * Custom table view
  * Detail screen
  * Labels
  
  
### The Controller
* View controllers—Control a view and its subviews
* Model controllers—Control  a collection of model objects
* Helper controllers—Consolidate related data or functionality that can be accessed by other objects

## Define Views and View Controllers
You've prototyped a workflow, or navigation hierarchy, that allows your user to access all the features you've imagined for your app. Take some time to plan out the view hierarchy and the view controller properties and methods for each scene. 

✏️ Answer the following questions:
* Does your workflow prototype provide access to every feature?
* What view objects will you use for each scene? What other options might you consider?
* What model objects will be displayed on each scene? For example, is it a list view that displays an array of model objects? * Or is it a detail view that shows a single instance?
* What `configure(_:)` or `updateUI(_:)` methods will you need for each view? What subviews will need to be updated with the model data displayed on the view?
* What other actions, such as fetching or saving data, may be added to a specific view controller?

Based on your prototype, write down the basic interface for each view controller, and list out the user interface elements for each scene. Add any properties for model objects and any helper methods you'll need on your view controllers to keep the interface updated correctly.

## Define Model or Helper Controllers

Although it's possible to build some (simple) apps using only view controllers, most apps benefit from model or helper controller types. Model controllers, for example, help keep track of your app's model data and typically handle persistence or network requests. Other controllers help you avoid packing too much code and clutter into your view controllers. It can also be useful to move functionality required by multiple view controllers and centralize it on a single helper controller.

✏️ Answer the following when identifying possible model or helper controllers for your app:

* What persistence or other potentially repeated tasks can be moved to a model controller?

* What tasks require complex code that may be better abstracted into a helper controller?

* Are there any other pieces of logic or code that may be broken into logical chunks of functionality under a separate controller?

## Check Against Your Feature List
At this stage, you'll want to review your prototype and feature list. Have you considered all the code you'll need to write for each step? Does your architecture plan reflect each feature? If you've missed a feature, revisit the previous steps and adjust your architecture plan to match.

Don't worry if you need to make adjustments. As the saying goes, no plan survives first contact with the enemy. It's extremely unlikely that you'll create a perfect project plan before you get into building the actual app. And as you start building and coding, you'll continue to make changes. Make sure to consider how each change affects the rest of your project plan—and take the time to go back and update the plan accordingly.

🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑 Submit Work to RCslatkin@syr.edu🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑🛑
## Build Your Project Plan
Now that you have an app architecture, create a plan for how you'll build the app. Your project plan will serve as your guide each time you sit down and work on the app.

Here's a general approach for building most apps:
1. Build out the workflows, or navigation hierarchy, for navigating the app in a storyboard.
2. Implement the model definitions and enter sample data.
3. Build the view hierarchies for each scene.
4. Implement the view controllers and wire the interface to the sample data.
5. Implement model and helper controllers.
6. Update the view controllers to create or use real data instead of sample data.
7. Polish the visual design, including colors, typography, and animation


## Create a Timeline 
Following a project plan of attack should result in a high-level overview of a working app. You can then implement each model object and scene, one at a time, while maintaining a demo-able experience that allows you to check your progress along the way. This incremental approach is far preferable to building pieces of the app separately and stitching them together at the very end—in the faint hope that everything will work as expected.

✏️ To create a project timeline, consider your own personal goals for the app and set some deadlines for achieving specific milestones. How can you estimate the time it will take for the steps above? Depending on the complexity of your app, each step will probably take longer than the previous step. In the prototyping lesson, your instructions were to imagine an app with no more than four screens. But you'll still find that building a four-screen app with one or two model objects will take many hours across days or weeks. Based on the projects in this course, do your best to come up with some rough completion timeframes that you feel you can commit to. 
