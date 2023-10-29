const axios = require('axios');

// Example function for making a GET request using Axios
async function fetchData() {
  try {
    const response = await axios.get('https://api.example.com/data');
    console.log(response.data);
  } catch (error) {
    console.error('Error fetching data:', error);
  }
}

// Example function for making a POST request using Axios
async function postData(data) {
  try {
    const response = await axios.post('https://api.example.com/post', data);
    console.log(response.data);
  } catch (error) {
    console.error('Error posting data:', error);
  }
}

// Call the functions
fetchData();
postData({ key: 'value' });

// You can add more functions for different types of requests
