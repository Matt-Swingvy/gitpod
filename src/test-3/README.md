# Manipulate leave balance history list

0. get response data from './leave_balance_histories.json'
1. Sort array by update date (latest first) (leaveBalanceHistory.updateDate)
2. Filter sorted array(result of #1) to 'Annual leave'.
3. Create leaveType map grouped by leaveType.id
4. Create list which type is Option[] from result of #3.
```
interface Option {
    value: number,
    title?: string,
}
```