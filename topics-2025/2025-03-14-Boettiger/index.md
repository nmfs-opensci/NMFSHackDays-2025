# Topic

**Author:** Carl Boettiger (UC Berkeley)



## Tutorials

Carl will be talking about integrating LLMs into data dashboards specifically this
[dashboard](https://huggingface.co/spaces/boettiger-lab/ca-30x30) ([source code](https://github.com/boettiger-lab/ca-30x30)).

**Use Carl's image**

When you start up the Jupyter Hub

1. Select Other for image
2. In the box, put `rocker/binder:latest`

**Clone Carl's demo repo**

```
cd ~
git clone https://github.com/boettiger-lab/geo-llm-r
```

**Carl's tutorial**

He went mainly through this example:

* https://github.com/boettiger-lab/geo-llm-r/blob/main/test.R

```
chat <- ellmer::chat_vllm(
  base_url = "https://llm.nrp-nautilus.io/",
  model = "llama3",
  api_key = "<token>"
)
```

