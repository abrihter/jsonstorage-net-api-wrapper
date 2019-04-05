# WRAPPER FOR JSONSTORAGE.NET API #
Simple wrapper for jsonstorage.net API, created by Alexander Doroshenko

## HOW TO USE ##
```Python
from b_wrapper_api_jsonstorage_net import bAPIWrapperJsonstorageNet

api = bAPIWrapperJsonstorageNet()

#create JSON object and get ID
object_id = api.create({'name': 'abrihter'})

if object_id:
	#load JSON object
	json_object = api.load(object_id)

	#update JSON object
	if api.update(object_id, {'name': 'bojan'}):
		print('JSON object updated!')
else:
	print('Extracting JSON object ID failed!')
```
