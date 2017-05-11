25/10/2016

Today I learned where to put my learning journal. as well as how to code movement referencing the input manager in unity.
(if (Input.GetAxisRaw("Horizontal") > 0) {
			// Move to the right
			transform.Translate (Vector3.right * Time.deltaTime);)
      
Input.GetAxisRaw("horizontal/vertical") references the input manager and axis,
transform.Translate (Vector3.right * Time.deltaTime);) references the movement and updates the forward face.

30/10/2016

Today I learned how to create a first person camera script using the mouse to control the view in game referencing the input manager in unity.
RotateX += HorizontalSpeed * Input.GetAxis("Mouse X"); 
RotateY-= VerticalSpeed * Input.GetAxis("Mouse Y"); References the mouse position in the input manager. 

transform.eulerAngles = new Vector3(RotateY, RotateX, 0.0f) Tacks the mouse position and updates the new camera position.

10/11/2016

I learned how to resize an object using "transform.localScale"  I then used this to replicate a player crouching by putting it into an "if" statement. this allows me to change and then reset the objects size.

18/11/2016

I learning how to activate UI on collision with an object then deactivating it after a certain amount of time, this was quite a challenge as I had not used UI before. I was learning about all of the components but fortunately it turned out to be fairly simple, all it needed was a "Public GameObject" and "OnCollision", as I had worked with tags prior to this I found the code fairly easy using the "SetActive" command I was able to toggle when the UI GameObject was visible just adding a simple count to deactivate it. 

22/11/2016

Today I learned how to link scripts together and how to active/deactivate them, I had decided this would be a nice system to use for a gaming health component. This proved to be a hard task due to the fact I couldn’t find a tutorial that could help me, after a while of searching one of my peers told me about the "GetComponent" code which allowed me to reference script thusly letting me use "setActive" in order to Turn it on and off. I then used a simple count and destroy to kill the player.

25/11/2016

As I had learned about "onCollisonEnter" last week I wanted to brush up on how to code an "OnTriggerEnter" Collisions as i had not done this in a long time. I needed this to allow an object to destroy another using tags, this was so I could differentiate between objects in the scene as to not accidently remove other assets. I had a little trouble with this as I had forgotten about the "is trigger" tab on the collider but once I had found this everything went smoothly.

1/12/2016

Today I created a rigidbody instantiation script, I had a lot of problems with this as I was struggling to find a comprehensive guide and once I had found one I found it relatively easy to write the base code. I was then having the issue of getting my object to have a force added to it as it was a child object (unity will only give a force if the object has a force itself) but once I had looked online for help I could add force to the object using "playerRotation = GetComponentInParent<Transform>();" which give the object the parents transform data. I then added a force to the instantiated object which i found fairly simple as it was included in the same guide.

28/2/2017

This task was to create a timer and for this I needed to learn how to reference and store the time and then how to display it using UI elements,  in order to create the trigger which should be death i created a simple collide with a trigger which then allows me to call the other script using "t = GameObject.FindGameObjectWithTag("DeadUI").GetComponent<Timer>();" this allows me to reference another script in the scene and then activate it. I found this incredibly tricky to do as I had no experience in this area but after researching I was able to find the simple code and implement it. The second script was a lot harder to make as I had never attempted to do this but after help from a student I was able to create a string which I could then reference and display using the UI.

7/3/2017

Today I had to improve my timer, to do this I simply created another string which could be referenced as minutes allowing for much more practical usage.

14/3/2017

For this task I created a simple Trigger, when a mouse button was pressed it would activate the collider which in turn would activate the destroy script.

21/3/2017

This week I was asked to create an instantiation script in order to place item's such as barricades, I thought this would be quite simple as all I needed was an instantiation script but tis will only create the object with the same translation underneath the character so in order to get around this I created an empty game object as a point of reference and generated the object on this so they will use the translate and rotation data of the parent (the character).

9/5/2017

Today I programed a moving platform, I created two empty objects to use as a marker for the platform to travel between, it was a little awkward but after playing with different speeds and learning how to use the correct referencing everything worked smoothly
