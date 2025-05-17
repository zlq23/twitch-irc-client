
### Usage
```
const twitchIRC = new TwitchIRC();

twitchIRC.on('message', (msg) => {
  console.log(msg);
  // msg.role => "broadcaster", "mod", "vip", "sub" or ""
  // msg.tags, msg.command, msg.params, etc.
});

twitchIRC.join('nervarien'); // Replace with your Twitch channel
```


### Message Object Example
```
{
  tags: {
    'display-name': 'SomeUser',
    'mod': '1',
    'subscriber': '0',
    // ...
  },
  prefix: 'someuser!someuser@someuser.tmi.twitch.tv',
  command: 'PRIVMSG',
  params: ['#channel', 'Hello world!']
}
```
