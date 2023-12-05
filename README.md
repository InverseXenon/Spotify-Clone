# Day 3

## CustomRange Component
- The primary function of the CustomRange component is to provide a user-friendly interface for seeking through a song's timeline.
- It plays a crucial role in enhancing the user experience when interacting with an audio player.
- Through callback functions, such as `onChange`, the CustomRange facilitates seamless integration with the audio element, allowing users to seek to specific positions in the playing song with ease.

## Voice Modulation
- Implementing voice modulation using the useVoiceModulation hook from the @specular-aura/voice-modulation library.
- It is integrated within the Player component to enhance audio playback.
- Voice modulation for the `megaphone` effect is implemented which can be triggered by the 'plus' icon button in the Player component.

## SongItem Component
- The SongItem component renders individual song items with a play button.
- It interacts with a global song context to handle playing the selected song when the play button is clicked.
- It accesses the global song context using the useContext hook.
- The playSong function sets the clicked song as the current song in the context, initiating playback with details such as artist, title, image, ID, and streaming URL for a seamless user experience in the SongItem component.

## Section Component
- The Section component is responsible for rendering a section of music content within the application's user interface.
- The Section component dynamically renders a section of music content with a specified title and a grid layout.
- The component provides an option for customizing the order of displayed items through the reverse prop.

## Home Page
- Within the Home component, the frontend renders the Section Component for music content display.
- Renders a section titled "Made For You" for personalized song recommendations.
- Utilizes mock data to stimulate recently played and recommended songs.

## Search Page
- The handleSearch function is responsible for executing the search logic based on the entered search term.
- The `useState` hook is used to manage the state of the search term (searchTerm) and search results (searchResults).
- `findIndex` method is used  to search for a matching song in the songs array within the global context.
- searchResults state gets updated with the matched songs or an empty array if there are no matches.
- Results Display Renders a grid of SongItem components for the matched search results.
- Each SongItem displays relevant information about the song and allows users to interact with it.

# Progress after Day 3
## Home Page
![The Home Page](frontend/screenshots/Day3-HomePage.png)

## Search Page
![The Home Page](frontend/screenshots/Day3-SearchPage.png)
