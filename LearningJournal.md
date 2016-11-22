25/10/2016

Today I learned where to put my learning journal. as well as how to code movement referencing the input manager in unity.
(if (Input.GetAxisRaw("Horizontal") > 0) {
			// Move to the right
			transform.Translate (Vector3.right * Time.deltaTime);)
      
Input.GetAxisRaw("horizontal/vertical") references the input manager and axis,
transform.Translate (Vector3.right * Time.deltaTime);) references the movement and updates the forward face.

30/10/2016

Today I learned how to create a first person camera script using the mouse to control the view in game refferancing the input manager in unity.
RotateX += HorizontalSpeed * Input.GetAxis("Mouse X"); 
RotateY-= VerticalSpeed * Input.GetAxis("Mouse Y"); Referances the mouse position in the input manager. 

transform.eulerAngles = new Vector3(RotateY, RotateX, 0.0f) Tacks the mouse position and updates the new camera position.

10/11/2016

I learned how to resize an object using "transform.localScale" i then usded this to replicate a player crouching by putting it into an "if" statement. this allows me to change and then reset the objects size.

18/11/2016

learning how to activate UI on collision with an object then deactivating it after a certain amout of time was quite a challange as i had not used UI before so i was learning about all of the componantes but fortunalty it turned out to be fairly simple all it needed was a "Public GameObject" and "OnCollision" as i had worked with tags priour to this i found the code fairly easy using the "SetActive" comand i was able to toggle when the UI GameObject was visible just adding a simple count to deactivate it. 
