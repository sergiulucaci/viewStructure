# viewStructure
This component consists needed structure for a view: the top nav bar, the bottom bar, the menu drawer and the body section. All sections can have children that can trigger actions, can be stylized, can be characterized by icons, etc. 

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
				topBarLeftButtonOnPress={() => this.navigateTo(‘home)}
				// Top bar - title
				topBarTitleButtonIcon={icon}
				topBarTitleText=“Home”
				topBarTitleStyle={styles.leftButtonStyle}
				// Top bar - right button
				topBarRightButtonIcon={leftIcon}
				topBarRightButtonText=“Back”	
				topBarRightButtonStyle={styles.leftButtonStyle}
				topBarRightButtonOnPress={() => this.navigateTo(‘otherView')}

				// Bottom bar - iOS
				bottomBar={true}
				bottomBarStyle={styles.barStyle}
				// Bottom bar - first button
				bottomBarFirstButtonIcon={leftIcon}
				bottomBarFirstButtonText=“Back”	
				bottomBarFirstButtonStyle={styles.leftButtonStyle}
				bottomBarFirstButtonOnPress={() => this.navigateTo(‘home)}
				// Bottom bar - secondButton,thirdButton, fourthButton - similar to first and second button. 
				// Maximum of buttons for bottom bar is 4. 
				// Menu button - iOS and Android
				menuDrawer={true}
				menuDrawerIcon={bottomMenuIcon}
				// Menu Button - children
				menuDrawerFirstChildText=“Home”
				menuDrawerFirstChildIcon={menuFirstChildIcon}
				menuDrawerFirstChildOnPress={() => this.navigateTo(‘home)}
				menuDrawerFirstChildStyle={styles.menuDrawerStyle}
			  // The next children for menu drawer (menuDrawer[Second, Third, Fourth++]ChildText) similar                                   with menuDrawerFirstChildText
			>
				// The body of the view
		</ViewStructure>
		)
	}
```
