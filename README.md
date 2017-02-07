# viewStructure
This component consists needed structure for a view: the top nav bar, the bottom bar, the menu drawer and the body section.  

Usage:
```
'use strict';
import React, { Component } from 'react';
import ViewStructure from 'view-structure';

class BasicView extends Component {
	render() {
		return (
			<ViewStructure 
				// Top bar - iOS and Android
				topBar={true}
				topBarStyle={styles.barStyle}
				// Top bar - left button
				topBarLeftButtonIcon={leftIcon}
				topBarLeftButtonText=“Back”	
				topBarLeftButtonStyle={styles.leftButtonStyle}
				// Top bar - title
				topBarTitleButtonIcon={icon}
				topBarTitleText=“Home”
				topBarTitleStyle={styles.leftButtonStyle}
				// Top bar - right button
				topBarRightButtonIcon={leftIcon}
				topBarRightButtonText=“Back”	
				topBarRightButtonStyle={styles.leftButtonStyle}

				// Bottom bar - iOS
				bottomBar={true}
				bottomBarStyle={styles.barStyle}
				// Bottom bar - first button
				bottomBarFirstButtonIcon={leftIcon}
				bottomBarFirstButtonText=“Back”	
				bottomBarFirstButtonStyle={styles.leftButtonStyle}
				// Bottom bar - second button
				bottomBarSecondButtonIcon={icon}
				bottomBarSecondText=“Home”
				bottomBarSecondStyle={styles.leftButtonStyle}	
				// Bottom bar - thirdButton, fourthButton - similar to first and second button. 
				// Maximum of buttons for bottom bar is 4. 
				// Menu button - iOS and Android
				menuDrawer={true}
				menuDrawerIcon={bottomMenuIcon}
				// Menu Button - children
				menuDrawerFirstChildText=“Home”
				menuDrawerFirstChildIcon={menuFirstChildIcon}
				menuDrawerFirstChildIconOnPress={() => this.navigateTo(‘home)}
			  // The next children for menu drawer (menuDrawer[Second, Third, Fourth++]ChildText) similar                                   with menuDrawerFirstChildText
			>
				// The body of the view
		</ViewStructure>
		)
	}
```
