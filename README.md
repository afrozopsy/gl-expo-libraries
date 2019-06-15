# gl-expo-libraries
Compilation of all up-to-date GL related libraries for react-native expo SDK.

## Usage

Download the tarbar and copy the contents in your project.
The you can import like, `import { GLImage , Surface } from gl-expo-libraries;`

-> I haven't created a package coz I thought it can make conflict with your downloaded(node_modules) libraries.

### Example Code

Below is the example,

`import React , { Component } from "react";
import { Container , Text } from 'native-base';
import { Surface , GLImage } from "./gl-expo-libraries";

export default class Example extends Component {
  render () {
    return (
     <Container>
      <Surface style={{ width: 300, height: 500 }}>
	        <GLImage
	          source={{ uri: 'http://i.imgur.com/zJIxPEo.jpg'}}
	          resizeMode="contain"
	        />		       	   		   	
      </Surface>  
      <Text>Java</Text>  	
     </Container>
    );
  }
}`


## SideNote,

Sole purpose of this repo is to make sure gl implementation of expo never breaks,
if you see changes that you think will make improvements then feel free to drop
a PR.