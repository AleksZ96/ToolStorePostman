Through API testing, I have identified an issue related to images. 
Specifically, the issue arises when attempting to add a new product and is associated with the "product_image_id" field. 
The request mandates it to be of type integer, while the IDs for all images accessible through the image retrieval endpoint are of type string.
Furthermore, I have observed a potential issue after creating a product, which is also linked to the ID. 
In this case, the product creation endpoint is expected to return a specific product in JSON format, containing an ID field of type integer. 
However, consistent with other products, this ID should ideally be of type string.
For instance, "id": "01HFYW9BK9N32B9CA0Q55K8RMW" cannot be translated to an integer, posing a potential source of error in the process.