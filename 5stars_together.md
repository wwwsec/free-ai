together.ai 提供免费的图片生成API,使用模型black-forest-labs/FLUX.1-schnell-Free


from together import Together

client = Together()
response = client.images.generate(
    prompt="[]",
    model="black-forest-labs/FLUX.1-schnell-Free",
    width=1024,
    height=768,
    steps=4,
    n=1,
    response_format="b64_json",
    stop=[]
)
print(response.data[0].b64_json)
