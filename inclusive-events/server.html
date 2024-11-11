const express = require('express');
const app = express();
const port = 5000; // Port where the server will run

// Middleware to parse JSON
app.use(express.json());

// Sample events data (JSON format)
let events = [
    {
        id: 1,
        title: "Black History Month Celebration",
        description: "A month-long celebration of Black history, culture, and contributions.",
        categories: ["Cultural", "Social Justice"],
        date: "2024-02-15",
        location: "Student Union Hall"
    },
    {
        id: 2,
        title: "Pride Week Kickoff",
        description: "A week dedicated to LGBTQ+ awareness and pride.",
        categories: ["LGBTQ+", "Social Justice"],
        date: "2024-06-01",
        location: "Campus Quad"
    },
    {
        id: 3,
        title: "Disability Awareness Workshop",
        description: "Workshop focused on accessibility and inclusion for students with disabilities.",
        categories: ["Accessibility", "Social Justice"],
        date: "2024-03-10",
        location: "Room 205, Admin Building"
    }
];

// Get all events
app.get('/events', (req, res) => {
    res.json(events);
});

// Filter events by category
app.get('/events/filter', (req, res) => {
    const { category } = req.query; // Get category from query string

    if (!category) {
        return res.status(400).json({ message: "Category is required" });
    }

    // Filter events by category
    const filteredEvents = events.filter(event => event.categories.includes(category));
    res.json(filteredEvents);
});

// Add a new event
app.post('/events', (req, res) => {
    const { title, description, categories, date, location } = req.body;

    if (!title || !description || !categories || !date || !location) {
        return res.status(400).json({ message: "Missing required fields" });
    }

    // Create new event
    const newEvent = {
        id: events.length + 1,
        title,
        description,
        categories,
        date,
        location
    };

    events.push(newEvent);
    res.status(201).json(newEvent);
});

// Update an event
app.put('/events/:id', (req, res) => {
    const { id } = req.params;
    const { title, description, categories, date, location } = req.body;

    const event = events.find(event => event.id === parseInt(id));

    if (!event) {
        return res.status(404).json({ message: "Event not found" });
    }

    // Update event fields
    event.title = title || event.title;
    event.description = description || event.description;
    event.categories = categories || event.categories;
    event.date = date || event.date;
    event.location = location || event.location;

    res.json(event);
});

// Delete an event
app.delete('/events/:id', (req, res) => {
    const { id } = req.params;

    const index = events.findIndex(event => event.id === parseInt(id));
    if (index === -1) {
        return res.status(404).json({ message: "Event not found" });
    }

    events.splice(index, 1);
    res.status(204).send(); // No content to return
});

// Start the server
app.listen(port, () => {
    console.log(`Server is running on port ${port}`);
});
