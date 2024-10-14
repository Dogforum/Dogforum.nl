<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dog Forum</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #e9ecef;
        }
        h1 {
            color: #343a40;
        }
        .forum-container {
            max-width: 800px;
            margin: auto;
            background: #ffffff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .category {
            margin: 10px 0;
            padding: 10px;
            background: #f8f9fa;
            border-radius: 5px;
        }
        .post {
            border-bottom: 1px solid #ccc;
            padding: 10px 0;
        }
        .post:last-child {
            border-bottom: none;
        }
        .post h2 {
            margin: 0;
            font-size: 1.5em;
        }
        .post p {
            margin: 5px 0;
            color: #555;
        }
        .emoji-reactions {
            margin-top: 10px;
        }
        .emoji {
            cursor: pointer;
            font-size: 20px;
            margin-right: 5px;
        }
        .reply-form {
            margin-top: 10px;
            display: none;
            background: #f8f9fa;
            padding: 10px;
            border-radius: 5px;
        }
        .reply {
            margin-left: 20px;
            padding: 5px;
            border-left: 2px solid #007BFF;
        }
        form {
            margin-top: 20px;
            background: #f8f9fa;
            padding: 15px;
            border-radius: 5px;
        }
        input[type="text"], textarea {
            width: 100%;
            padding: 10px;
            margin: 5px 0 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        input[type="file"] {
            margin: 5px 0 15px;
        }
        input[type="submit"] {
            background-color: #007BFF;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 4px;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #0056b3;
        }
        .search-bar {
            margin-bottom: 20px;
            position: relative;
        }
        .suggestions {
            position: absolute;
            background: white;
            border: 1px solid #ccc;
            width: 100%;
            z-index: 10;
        }
        .suggestion-item {
            padding: 10px;
            cursor: pointer;
        }
        .suggestion-item:hover {
            background-color: #f1f1f1;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="forum-container">
        <h1>Dog Forum</h1>

        <div class="search-bar">
            <input type="text" placeholder="Search for dog breeds..." id="search-input" onkeyup="showSuggestions(this.value)">
            <input type="submit" value="Search" onclick="searchBreed()">
            <div class="suggestions" id="suggestions-list"></div>
        </div>

        <h2>Categories</h2>

        <div class="category">
            <h3>Labrador Retriever</h3>
            <p>Labrador Retrievers are known for their friendly nature and intelligence...</p>
        </div>
        <!-- Add other breed categories here as before -->

        <div class="post">
            <h2>Welcome to the Dog Forum!</h2>
            <p>Share your experiences, tips, and stories about dogs.</p>
        </div>

        <form id="post-form">
            <h3>Start a New Topic</h3>
            <input type="text" placeholder="Topic Title" required>
            <textarea placeholder="Your message..." rows="4" required></textarea>
            <input type="file" accept="image/*" id="image-input">
            <input type="submit" value="Post">
        </form>
    </div>

    <script>
        const breeds = [
            "Labrador Retriever", "German Shepherd", "Beagle", "Bulldog",
            "Golden Retriever", "Poodle", "French Bulldog", "Rottweiler",
            "Yorkshire Terrier", "Dachshund", "Boxer", "Siberian Husky",
            "Shih Tzu", "Great Dane", "Chihuahua", "Corgi", "Doberman Pinscher"
        ];

        function showSuggestions(value) {
            const suggestionsList = document.getElementById('suggestions-list');
            suggestionsList.innerHTML = '';

            if (!value) return;

            const filteredBreeds = breeds.filter(breed => breed.toLowerCase().startsWith(value.toLowerCase()));

            filteredBreeds.forEach(breed => {
                const item = document.createElement('div');
                item.className = 'suggestion-item';
                item.textContent = breed;
                item.onclick = () => {
                    document.getElementById('search-input').value = breed;
                    suggestionsList.innerHTML = '';
                };
                suggestionsList.appendChild(item);
            });
        }

        function searchBreed() {
            const input = document.getElementById('search-input').value.toLowerCase();
            let closestMatch = '';

            breeds.forEach(breed => {
                if (breed.toLowerCase() === input) {
                    closestMatch = breed; // Exact match found
                } else if (breed.toLowerCase().includes(input)) {
                    closestMatch = breed; // Fuzzy match found
                }
            });

            if (closestMatch) {
                alert(`You searched for: ${closestMatch}`);
            } else {
                alert('No matching breed found. Please check your spelling.');
            }
        }

        function addReaction(postElement, emoji) {
            const reactionDiv = postElement.querySelector('.reaction-count');
            reactionDiv.textContent = parseInt(reactionDiv.textContent || '0') + 1;
        }

        function toggleReplyForm(postElement) {
            const replyForm = postElement.querySelector('.reply-form');
            replyForm.style.display = replyForm.style.display === 'block' ? 'none' : 'block';
        }

        function addReply(postElement, event) {
            event.preventDefault();
            const replyText = postElement.querySelector('.reply-input').value;
            const replyContainer = postElement.querySelector('.replies');

            const newReply = document.createElement('div');
            newReply.className = 'reply';
            newReply.innerHTML = `<p>${replyText}</p>`;
            replyContainer.appendChild(newReply);
            postElement.querySelector('.reply-input').value = ''; // Clear input
        }

        document.getElementById('post-form').onsubmit = function(event) {
            event.preventDefault();
            const imageInput = document.getElementById('image-input');
            if (imageInput.files && imageInput.files[0]) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const newPost = document.createElement('div');
                    newPost.className = 'post';
                    newPost.innerHTML = `
                        <h2>New Post</h2>
                        <p>${event.target[0].value}</p>
                        <p>${event.target[1].value}</p>
                        <img src="${e.target.result}" alt="Dog Image">
                        <div class="emoji-reactions">
                            <span class="emoji" onclick="addReaction(this.parentNode.parentNode, '😊')">😊</span>
                            <span class="emoji" onclick="addReaction(this.parentNode.parentNode, '❤️')">❤️</span>
                            <span class="emoji" onclick="addReaction(this.parentNode.parentNode, '👍')">👍</span>
                            <span class="emoji" onclick="addReaction(this.parentNode.parentNode, '😂')">😂</span>
                            <span class="reaction-count"></span>
                        </div>
                        <button onclick="toggleReplyForm(this.parentNode)">Reply</button>
                        <div class="reply-form">
                            <input type="text" placeholder="Your reply..." class="reply-input" required>
                            <input type="submit" value="Post Reply" onclick="addReply(this.parentNode.parentNode, event)">
                        </div>
                        <div class="replies"></div>
                    `;
                    document.querySelector('.forum-container').appendChild(newPost);
                    event.target.reset(); // Reset the form
                };
                reader.readAsDataURL(imageInput.files[0]);
            }
        };
    </script>
</body>
</html>
