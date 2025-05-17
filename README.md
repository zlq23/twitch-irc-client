
### Usage
```
const twitchIRC = new TwitchIRC();

twitchIRC.on('message', (msg) => {
  console.log(msg);
  // msg.tags.role => "broadcaster", "mod", "vip", "sub" or ""
  // msg.tags, msg.command, msg.params, etc.
});

twitchIRC.join('channel'); // Replace with twitch channel
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
