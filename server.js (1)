require('dotenv').config();
const express = require('express');
const cors = require('cors');

const app = express();
app.use(cors());
app.use(express.json());

// Main Resolution Endpoint
app.post('/resolve', async (req, res) => {
    const { domain } = req.body;
    console.log(`Resolving: ${domain}`);

    // Placeholder: This is where we will hook into your 
    // database later to return the true owner.
    res.json({
        domain: domain,
        status: "success",
        owner: "0x000...placeholder",
        message: "Legacy Platform Resolver Active"
    });
});

const PORT = process.env.PORT || 3000;
app.listen(PORT, () => console.log(`The Legacy Platform live on port ${PORT}`));
