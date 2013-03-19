JSAnnotations
=============

This allows you to develop annotation-based JavaScript-Code.

### Example:

This example:

	function Car(name) {

		//@Pr�fix{"foo_"}
		this.name = name;

	}

will result in this object:

	{
		annotations: [
			0: {
				annotation: "Pr�fix",
				parameters: [
					0: "foo_"
				]
			}
		],
		object: "this.name = name;"
	}