# ERROR DOCUMENTATION
Here will all my error documentation and how to solve them

## Index

  - [Table Of contents](#index)
    - [React router doesn't work in firebase production servers (Showing cannot get /route)](#react-router-doesnt-work-in-firebase-production-servers-showing-cannot-get-route)




### React router doesn't work in firebase production servers (Showing cannot get /route)

Got some hints to solve this from seeing this 
[article](https://ui.dev/react-router-cannot-get-url-refresh/)

either way checkout the firebase docs, and "find rewrite under firebase hosting" and do this, 
`
"rewrites": [
			{
				"source": "**",
				"destination": "/index.html",
				"function": "app"
			}
		],
`
It will redirect the Page to it's desired location.