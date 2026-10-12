# TechFest Pune – Event Registration

A ReactJS web application for registering for a college tech fest. It demonstrates client-side form validation and an interactive user experience.

**Live demo:** https://SwaraliNasikkar.github.io/techfest-registration/

## Features
- Registration form with name, email, mobile number, event, tickets, promo code and rules checkbox
- Real-time client-side validation with specific error messages
- Success feedback on valid fields and a confirmation message after submission
- Error summary on invalid submit, with focus moved to the first invalid field
- Live ticket preview and total price that update as you type
- Promo codes (`STUDENT10`, `EARLY20`) with discount calculation
- Registrations list with a cancel option
- Light and dark theme toggle
- Responsive layout and accessible labels

## Validation Rules
| Field | Rule |
|---|---|
| Name | Required, 3–50 characters, letters only |
| Email | Required, valid email format |
| Mobile | Required, exactly 10 digits, starts with 6–9 |
| Event | Must be selected |
| Tickets | Between 1 and 5 |
| Promo code | Optional, must be a valid code |
| Rules | Checkbox must be ticked |

## React Concepts Used
- Function components (`App`, `Field`)
- State with `useState`, and `useRef` to focus the first error
- Event handling: `onInput`, `onBlur`, `onChange`, `onSubmit`
- Conditional rendering and list rendering with keys
- A reusable validation function

## Tech Stack
React 18 (via CDN), HTML5, CSS3, JavaScript (ES6)

## How to Run
1. Download or clone this repository.
2. Open `index.html` in a browser.

## Test Cases
| Input | Result |
|---|---|
| Name `Ab` or `Rahul123` | Error shown |
| Email `rahul@` | Invalid email error |
| Phone `12345` | Length error |
| Promo `ABC` | Invalid promo error |
| Promo `STUDENT10` | 10% discount applied |
| Checkbox unticked | Rules error |
| All fields valid | Confirmation message and entry added to the list |
