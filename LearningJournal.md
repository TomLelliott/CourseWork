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
