1) download ip-adaptor.bin file and keep it in 
        C:\Users\Piyush Kumar\AppData\Local\Comfy-Desktop\ComfyUI-Shared\models\instantid

2) open load instantId model  -> ip-adaptor.bin must be in that

3) open Load instant Id face analysis -> cpu,cuda

4) open Load controller_net_model -> instantId\defusion_pytorch_model.safetensors

5) open batch iamge -> for multiple image

6) open apply instant id :-
                        1) instantId -> mapped with ( Load isnatnt id model ) 
                        2) insightface -> mapped with ( instant Id face analysis)
                        3) controll net -> load control_net_model
                        4) image -> input image
                        5) model -> actual diffusion model (text to image)
                        6) image_kps (key point images) -> only guide the face pose (angle postion the face)
                        7) weight -> how much output follow (1.0)
                        8) start_at -> begin
                        9) end_at -> end

7)  ksampler :-
                        1) sampler_name -> dpmpp_2m
                        2) schedular -> karras                