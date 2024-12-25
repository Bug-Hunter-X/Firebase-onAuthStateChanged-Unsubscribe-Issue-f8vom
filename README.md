# Firebase onAuthStateChanged Unsubscribe Issue
This repository demonstrates a common issue with Firebase's onAuthStateChanged function: improper unsubscription.  The provided code snippets show the problematic scenario and a corrected version.

## Problem
The original `onAuthStateChanged` listener isn't properly unsubscribed, which can lead to memory leaks, unexpected behavior, and potential errors.

## Solution
The solution ensures that the listener is unsubscribed when it's no longer needed (e.g., when a component unmounts in a React application).  This prevents resource exhaustion and maintains application stability.