25/10/2016

Today I learned where to put my learning journal. as well as how to code movement referencing the input manager in unity.
(if (Input.GetAxisRaw("Horizontal") > 0) {
			// Move to the right
			transform.Translate (Vector3.right * Time.deltaTime);)
      
Input.GetAxisRaw("horizontal/vertical") references the input manager and axis,
transform.Translate (Vector3.right * Time.deltaTime);) references the movement and updates the forward face.


