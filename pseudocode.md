# Weather App

Objects:
    Main Container - a <div> that holds all the page elements
    Input Field - a form element that lets a user input a zip code
    Submit Button - a button that on click takes the zip code input, retrieves the weather info from the API, and initializes the creation of the rest of the page elements

Functions:
    layoutCreation - a looping function that creates a row with a column appended and appends it to the main container

        function addNew() {
            for (let i = 0, i <= x; i++) // x is the number of times to run the loop
            const newDiv-R(i) = document.createElement('div');
            newDiv-R(i).setAttribute('class', row)
            newDiv-R(i).setAttribute('id', row-(i))
            document.container.appendChild(newDiv-R(i));
            const newDiv-(i)c = document.createElement('div');
            newDiv-C(i).setAttribute('class', col)
            newDiv-C(i).setAttribute('id', col-(i))
            document.newDiv-R(i).appendChild(newDiv-C(i));
        }

    render - takes the info from the JSON file (obtained from the API) and inserts it into the corresponding elements of the HTML document


## Program Start
    INIT on load
        CREATE main container <div>
        CREATE app title <h1>
        CREATE input field for zip code <form>
        CREATE submit button <button>

    On button click
        RUN  layoutCreation function
        FETCH the info from the API based on the zip code that the user input
        RUN the render function