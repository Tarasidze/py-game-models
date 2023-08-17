Game Models for a Django-based Game
Description

The Game Models for a Django-based Game project involves the development of crucial database models necessary for a game using the Django web framework. The primary focus is on creating a solid foundation for player interactions within the game world. This includes the ability for players to choose distinct races, each with their own unique set of skills, as well as the option to join guilds. By implementing these fundamental models, the project aims to facilitate core gameplay mechanics and features.
Technology Used

    Python
    Django

Components
Race Model

Players are provided with a variety of races to select from, such as Elf, Dwarf, Human, or Ork. The Race model is structured to encompass these race options, with the following attributes:

    name: A unique character field allowing a maximum of 255 characters to store the name of the race.
    description: A text field that can be left blank, intended to provide additional information about the race.

Skill Model

Each race possesses a distinct set of skills that contribute to the gameplay experience. The Skill model encapsulates these skills, featuring the following properties:

    name: A unique character field, allowing up to 255 characters for the name of the skill.
    bonus: A character field with a maximum length of 255 characters, describing the benefits that players can acquire from the skill.
    race: A foreign key reference to the Race model, establishing a link between skills and the races that possess them.

Guild Model

The game provides players with the opportunity to affiliate themselves with various guilds, fostering community and cooperation. The Guild model represents these guilds and includes the following attributes:

    name: A unique character field allowing a maximum of 255 characters to store the guild's name.
    description: A text field that can be left blank, providing a brief overview of the guild.

Player Model

At the core of player interaction lies the Player model, which captures individual player information and choices. The model encompasses the following properties:

    nickname: A unique character field with a maximum length of 255 characters, representing the player's chosen nickname.
    email: An email field with a maximum length of 255 characters, facilitating communication with players.
    bio: A character field allowing up to 255 characters, providing a concise player-provided self-description.
    race: A foreign key reference to the Race model, indicating the player's selected race.
    guild: A foreign key reference to the Guild model, storing the ID of the player's associated guild. Importantly, player data remains intact even if the guild is deleted.
    created_at: A DateTime field set to the current time by default, capturing the player's registration timestamp.

Project Tasks

The project is divided into tasks, each contributing to the overall completion of the game models. Detailed tasks can be found in the project's documentation.
Checklist

Before submitting your solution, make sure to review the provided checklist to ensure that all project aspects are in order.

This project serves not only as the backbone for the game's mechanics but also as a practical example of Django's model system and its ability to shape and manage critical gameplay elements.
