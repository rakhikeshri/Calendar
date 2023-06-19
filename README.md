// // way 1 for finding leap year --------------------------------------
// // function isLeapYear(year) {
// //   // Check if the year is evenly divisible by 4
// //   if (year % 4 === 0) {
// //     // If the year is divisible by 100, check if it's also divisible by 400
// //     if (year % 100 === 0) {
// //       if (year % 400 === 0) {
// //         return true; // Divisible by 400, so it's a leap year
// //       } else {
// //         return false; // Divisible by 100 but not by 400, not a leap year
// //       }
// //     } else {
// //       return true; // Divisible by 4 but not by 100, so it's a leap year
// //     }
// //   } else {
// //     return false; // Not divisible by 4, not a leap year
// //   }
// // }

// // // Example usage
// // const year = 2024;
// // if (isLeapYear(year)) {
// //   console.log(year + " is a leap year.");
// // } else {
// //   console.log(year + " is not a leap year.");
// // }

// // way 2 for finding leap year -----------------------------------------
// // let leap_year_or_not;
// // const lear_year = (year) => {
// //   if(year % 4 === 0 && year % 100 != 0){
// //     leap_year_or_not = year + ' is a leap year'
// //   }else if(year % 100 === 0 && year % 4 === 0 && year % 400 === 0){
// //     leap_year_or_not = year + ' is a leap year'
// //   }else{
// //     leap_year_or_not = year + ' is not a leap year'
// //   }

// //   return leap_year_or_not
// // }


// /* lear_year(current_date.getFullYear()) === true ? "true" : "false"} <br /> */

// function App() {
//   const [year, setYear] = useState(null);
//   const [isLeapYear, setIsLeapYear] = useState(false);

//   //finding leap year
//   let current_year;
//   const leap_year = (year) => {
//     if (year % 4 === 0 && year % 100 !== 0) {
//       return true;
//     } else if (year % 100 === 0 && year % 4 === 0 && year % 400 === 0) {
//       return true;
//     } else {
//       return false;
//     }
//   };

//   useEffect(() => {
//     current_year = new Date().getFullYear();
//     setYear(current_year);

//     if (leap_year(current_year)) {
//       setIsLeapYear(true);
//     } else {
//       setIsLeapYear(false);
//     }
//   }, []);
