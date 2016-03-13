# node-red-contrib-leveldb-hyper-ttl

This fork of node-red-contrib-leveldb-ttl just adds live backup functionality via a new level-ttl backup node. This is done by using the alternate level-hyper package which has live backup built in.

See leveldown-hyper for more details:
https://github.com/level/leveldown-hyper

##Install

Run the following command in the root directory of your Node-RED install

    npm install node-red-contrib-leveldb-hyper-ttl
   
    or

    npm install git://github.com/jonn26/node-red-contrib-leveldb-hyper-ttl.git



##Usage of backup node

Use this node to perform a <b>live backup</b> of the database. The <b>name</b> parameter is a String. A successful live backup will result in a backup folder named backup-:<b>name</b> inside the location folder of the current database. The backup name can be set by the <b>msg.payload</b> or in the properties of this node which overrides anything specified in the <b>msg.payload</b>.

##Usage of the other leveldb nodes

See: https://github.com/min0n/node-red-contrib-leveldb-ttl
