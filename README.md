<!---
 license: Licensed to the Apache Software Foundation (ASF) under one
         or more contributor license agreements.  See the NOTICE file
         distributed with this work for additional information
         regarding copyright ownership.  The ASF licenses this file
         to you under the Apache License, Version 2.0 (the
         "License"); you may not use this file except in compliance
         with the License.  You may obtain a copy of the License at

           http://www.apache.org/licenses/LICENSE-2.0

         Unless required by applicable law or agreed to in writing,
         software distributed under the License is distributed on an
         "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
         KIND, either express or implied.  See the License for the
         specific language governing permissions and limitations
         under the License.
-->

# org.apache.cordova.contacts

Plugin documentation: [doc/index.md](doc/index.md)


---


##Changes:

###Contact Photos

Get base64 encoded contact photos instead of urls by modifying the `option` object.

    var options = new ContactFindOptions();  
    options.photoBase64 = true;


You can also store contact photos with base64 encoded images.

    var contact = navigator.contacts.create();
    
	var photos = [];
    photos[0] = new ContactField('base64', '9oADAMBAAIRAxEA...', false);
    
	contact.save();

	
Supported platforms: android

