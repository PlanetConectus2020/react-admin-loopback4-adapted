#Intro Loopback 4 provider for react-admin.

Correct some files to adapt LoopBack4 to REACT Admin 

#Usage npm -i react-admin-loopback4-adapted

import React, { Component } from 'react';
import { Admin, Resource, ListGuesser } from 'react-admin';
import lb4Provider from 'react-admin-lb4';

class MyComponent extends Component {
  render() {
    return (
        <Admin dataProvider={lb4Provider('http://localhost:3000')}>
          <Resource name="resource" list={ListGuesser} />
        </Admin>
    );
  }
