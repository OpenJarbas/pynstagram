# Pynstagram

Python Instagram API

## Install

```bash
pip install pynstagram
```

## Usage

```python
import pynstagram

user = "futurismcartoons"

profile_picture = pynstagram.get_profile_pic(user)

print(profile_picture)

```

    {'created_time': 1286323200,
     'shortcode': '',
     'urls': ['https://instagram.fopo2-1.fna.fbcdn.net/v/t51.2885-19/s150x150/24175725_782070811984521_1892833675515527168_n.jpg?_nc_ht=instagram.fopo2-1.fna.fbcdn.net&_nc_ohc=YRQK7qx5X_oAX-XX58o&oh=950f5811b378707afb7d88988c5dd1c0&oe=5F54C683'],
     'username': 'futurismcartoons'}

```python
import pynstagram

user = "futurismcartoons"

for media in pynstagram.get_media(user, comments=True):
    print(media)
```

    {'comments': [{'created_at': 1570550912,
               'id': '17844687733706431',
               'owner': {'id': '3662580333',
                         'profile_pic_url': 'https://instagram.fopo2-1.fna.fbcdn.net/v/t51.2885-19/s150x150/107337740_797731733964316_2261891563802277869_n.jpg?_nc_ht=instagram.fopo2-1.fna.fbcdn.net&_nc_ohc=pwg0odhLOxUAX_zYa_o&oh=ec071c552bcc5fe053487bf1f13c2370&oe=5F5678C1',
                         'username': 'nde.great'},
               'text': 'Bold of you to assume we need books to read'},
              {'created_at': 1570551455,
               'id': '17918065825338733',
               'owner': {'id': '1721319143',
                         'profile_pic_url': 'https://instagram.fopo2-1.fna.fbcdn.net/v/t51.2885-19/s150x150/75366272_2441967582518285_5384076491510251520_n.jpg?_nc_ht=instagram.fopo2-1.fna.fbcdn.net&_nc_ohc=DWRAM8BsCtEAX-7F6sM&oh=6dfb52eb76b8170a2c86f19e40fef986&oe=5F581048',
                         'username': 'miguelmed1'},
               'text': "What's the thing on the top of the girl's tablet?"},
               
             (...)
             
              {'created_at': 1596359028,
               'id': '17854637777110405',
               'owner': {'id': '4707133986',
                         'profile_pic_url': 'https://instagram.fopo2-1.fna.fbcdn.net/v/t51.2885-19/s150x150/91908859_155240155730797_5144424686557331456_n.jpg?_nc_ht=instagram.fopo2-1.fna.fbcdn.net&_nc_ohc=HSEmW1YBhgIAX_aNCeA&oh=df31a0cd56cbc84efe03b3b520e2eba1&oe=5F547157',
                         'username': 'mr.ugurcevik'},
               'text': '✅👍'}],
     'dimensions': {'height': 1080, 'width': 1080},
     'item_id': '2150258449741806801',
     'tags': ['automation',
              'comic',
              'arcade',
              'racing',
              'technology',
              'videogames',
              'games',
              'cartoons',
              'machinelearning',
              'raceday',
              'futurism',
              'pollposition',
              'futurismcartoons',
              'future',
              'science',
              'futurismdraws',
              'AI'],
     'text': 'Accelerating the advent of autonomous racing. \u2060\n'
             '\u2060\n'
             '\u2060See more futuristic cartoons like this one in our book '
             '"Cartoons from Tomorrow" available now at the link in bio. \u2060\n'
             '\u2060\n'
             'Comic by @lukekingma and @loupatrickmackay \u2060\n'
             '\u2060\n'
             '\u2060#futurismcartoons #futurismdraws #futurism #science '
             '#automation #AI #machinelearning #arcade #games #pollposition '
             '#racing #raceday #future #technology #videogames #comic #cartoons',
     'ts': 1570550803,
     'url': 'https://instagram.fopo2-1.fna.fbcdn.net/v/t51.2885-15/e35/70694853_759620494490135_892754774143256178_n.jpg?_nc_ht=instagram.fopo2-1.fna.fbcdn.net&_nc_cat=111&_nc_ohc=jaTJ9SDko6QAX8tKdcP&se=8&oh=91349805e08560e020306fcad4062f0d&oe=5F57DED1&ig_cache_key=MjE1MDI1ODQ0OTc0MTgwNjgwMQ%3D%3D.2',
     'username': 'futurismcartoons'}
