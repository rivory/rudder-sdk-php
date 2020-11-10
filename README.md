# What is RudderStack?

**Short answer:**
Rudder is an open-source Segment alternative written in Go, built for the enterprise. .

**Long answer:**
Rudder is a platform for collecting, storing and routing customer event data to dozens of tools. Rudder is open-source, can run in your cloud environment (AWS, GCP, Azure or even your data-centre) and provides a powerful transformation framework to process your event data on the fly.

## Getting Started with Python SDK

Install `rudder-sdk-php` using `composer`
```
git clone https://github.com/rudderlabs/rudder-sdk-php /my/app/folders/
```

## Initialize the ```Client```
```
Rudder::init(WRITE_KEY, array(
  "data_plane_url" => DATA_PLANE_URL,
  "consumer"       => "lib_curl", // fork_curl
  "debug"          => true,
  "max_queue_size" => 10000,
  "batch_size"     => 100
));
```

## Send Events
```
Rudder::track(array(
  "userId" => "f4ca124298",
  "event" => "Signed Up",
  "properties" => array(
    "plan" => "Enterprise"
  )
));
```

## Contact Us
If you come across any issues while configuring or using RudderStack, please feel free to [contact us](https://rudderstack.com/contact/) or start a conversation on our [Discord](https://discordapp.com/invite/xNEdEGw) channel. We will be happy to help you.
