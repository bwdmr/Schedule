# Scheduler


## About
A headless calendar component.
Features:
  - origin day
  - day view
  - monthly view
  - yearly view
  - select single
  - deselect single
  - select range
  - deselect range
  - toggle
  - detect floor
  - detect ceil
  - detect pole 
  - set schedule within day

and many more...


## Usage
```tsx
const { calendar } = useSchedule({ numberOfMonths: 1 })
...
{calendar.map((month) => {
  ...
  {month.map((week, weekIdx) => {
    const weekDayMap = week[1];
    const weekDayArray = [...weekDayMap];

    {weekDayArray.map((dayTouple, dayIdx) => {
      const day = dayTouple[0];
      let schedule = dayTouple[1];
      ...
    })}
  })}
})}
```

