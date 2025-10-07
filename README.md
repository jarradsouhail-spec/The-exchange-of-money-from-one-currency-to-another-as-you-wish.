# The-exchange-of-money-from-one-currency-to-another-as-you-wish.
The exchange of money from one currency to another as you wish.
New Chat
106 lines

const API_KEY = 'YOUR_API_KEY'; // Get free from exchangerate-api.com
const API_BASE = 'https://v6.exchangerate-api.com/v6/';
// Elements
const amountInput = document.getElementById('amount');
const fromSelect = document.getElementById('fromCurrency');
const toSelect = document.getElementById('toCurrency');
const swapBtn = document.getElementById('swapBtn');
const convertBtn = document.getElementById('convertBtn');
const resultDiv = document.getElementById('result');
const convertedP = document.getElementById('convertedAmount');
const rateP = document.getElementById('rateInfo');
const fromSym = document.getElementById('fromSym');
const toSym = document.getElementById('toSym');
const rateSpan = document.getElementById('rate');
const historyBtn = document.getElementById('historyBtn');
const chartContainer = document.getElementById('chartContainer');
const darkToggle = document.getElementById('darkModeToggle');
// Dark Mode Toggle
darkToggle.addEventListener('click', () => {
    document.body.classList.toggle('dark-mode');
    const icon = darkToggle.querySelector('i');
    icon.classList.toggle('fa-moon');
    icon.classList.toggle('fa-sun');
});
// Swap Currencies

