Public Toilets App
Form to submit a toilet
Form fields

    City (select) city required, minlength 3
    zip code (text) zip required, minlength 5, maxlength 5
    Street (text) street required, minlength 3
    House Nr. (text) streetnr required
    Name of location (text) name
    Features
        Mirror (checkbox) feat-mirror
        Paper towels (checkbox) feat-papertowels
        Perfume (checkbox) feat-perfume
        Accessibility (text) feat-access
        Soap (checkbox) feat-soap
    Number of stalls (number) stalls
    Rating (1 - 5 toilet seats) (radio group) rating (Number) required, min 1, max 5

Form styling

    Add custom focus styling for form fields
    Make the checkboxes appear as switches
    Make the rating radio boxes appear as stars or toilet seats (https://codepen.io/neilpomerleau/pen/wzxzQr)

List of submissions

    Table view
    Column for each Form field
    Column titles


List of submissions

    Table view
    Column for each Form field
    Column titles

Load form data

    Insert this code at the end of the html document that contains the table:

<script src="https://kloapp.herokuapp.com/javascripts/pure.min.js"></script>
<script src="https://kloapp.herokuapp.com/javascripts/render.js"></script>

    Your table needs to have the id toilets-table
    The part of your table that will hold the toilet data needs to be inside of a tbody tag
    The data will be assigned according to classes. Make sure that your table has one row with columns(td) that have the following classes:
        td.city
        td.location
        td.address
        td.feat-mirror
        td.feat-papertowels
        td.feat-perfume
        td.feat-access
        td.feat-soap,
        td.stalls,
        td.rating
    The data will only be added if all the classes are present
