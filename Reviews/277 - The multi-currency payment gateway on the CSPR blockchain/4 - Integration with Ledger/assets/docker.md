```
Sending build context to Docker daemon     568B

Step 1/7 : FROM node:lts
lts: Pulling from library/node

[1A[2K
b281ebec60d2: Pulling fs layer 
[1B
[1A[2K
74dae484504b: Pulling fs layer 
[1B
[1A[2K
21739e3ef21a: Pulling fs layer 
[1B
[1A[2K
e98d6bb51c7c: Pulling fs layer 
[1B
[1A[2K
517ebafd9747: Pulling fs layer 
[1B
[1A[2K
fa245e9d6fa2: Pulling fs layer 
[1B
[1A[2K
662bb10a8d17: Pulling fs layer 
[1B
[1A[2K
fad28b720f14: Pulling fs layer 
[1B
[1A[2K
512c94f3667e: Pulling fs layer 
[1B[6A[2K
e98d6bb51c7c: Waiting 
[6B[5A[2K
517ebafd9747: Waiting 
[5B[4A[2K
fa245e9d6fa2: Waiting 
[4B[1A[2K
512c94f3667e: Waiting 
[1B[3A[2K
662bb10a8d17: Waiting 
[3B[2A[2K
fad28b720f14: Waiting 
[2B[7A[2K
21739e3ef21a: Downloading [>                                                  ]  101.8kB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [>                                                  ]  81.67kB/7.856MB
[8B[8A[2K
74dae484504b: Downloading [=>                                                 ]  163.1kB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [=>                                                 ]  310.5kB/9.997MB
[7B[7A[2K
21739e3ef21a: Downloading [====>                                              ]  883.1kB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [===>                                               ]  510.3kB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [=====>                                             ]  1.112MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [====>                                              ]  674.2kB/7.856MB
[8B[8A[2K
74dae484504b: Downloading [====>                                              ]  756.1kB/7.856MB
[8B[9A[2K
b281ebec60d2: Downloading [>                                                  ]  506.2kB/50.44MB
[9B[7A[2K
21739e3ef21a: Downloading [=========>                                         ]  1.915MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [=======>                                           ]  1.178MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [================>                                  ]  3.292MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [=========>                                         ]  1.506MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [====================>                              ]  4.082MB/9.997MB
[7B[9A[2K
b281ebec60d2: Downloading [=>                                                 ]  1.014MB/50.44MB
[9B[7A[2K
21739e3ef21a: Downloading [=======================>                           ]   4.77MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [===========>                                       ]  1.751MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [===========================>                       ]   5.45MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [=============>                                     ]  2.087MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [==============================>                    ]  6.134MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [===============>                                   ]  2.423MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [==================================>                ]  6.822MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [=================>                                 ]  2.751MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [====================================>              ]  7.388MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [===================>                               ]  2.997MB/7.856MB
[8B[9A[2K
b281ebec60d2: Downloading [=>                                                 ]  1.534MB/50.44MB
[9B[7A[2K
21739e3ef21a: Downloading [=======================================>           ]  7.961MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [=====================>                             ]  3.419MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [===========================================>       ]  8.764MB/9.997MB
[7B[8A[2K
74dae484504b: Downloading [========================>                          ]  3.828MB/7.856MB
[8B[7A[2K
21739e3ef21a: Downloading [===============================================>   ]  9.567MB/9.997MB
[7B[7A[2K
21739e3ef21a: Verifying Checksum 
[7B[7A[2K
21739e3ef21a: Download complete 
[7B[8A[2K
74dae484504b: Downloading [===========================>                       ]  4.246MB/7.856MB
[8B[8A[2K
74dae484504b: Downloading [==============================>                    ]  4.737MB/7.856MB
[8B[8A[2K
74dae484504b: Downloading [==================================>                ]  5.479MB/7.856MB
[8B[9A[2K
b281ebec60d2: Downloading [==>                                                ]   2.05MB/50.44MB
[9B[8A[2K
74dae484504b: Downloading [=======================================>           ]   6.22MB/7.856MB
[8B[8A[2K
74dae484504b: Downloading [=============================================>     ]  7.207MB/7.856MB
[8B[8A[2K
74dae484504b: Verifying Checksum 
[8B[8A[2K
74dae484504b: Download complete 
[8B[9A[2K
b281ebec60d2: Downloading [==>                                                ]  2.558MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [>                                                  ]  530.8kB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [===>                                               ]  3.066MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [==>                                                ]  2.108MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [===>                                               ]  3.152MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [===>                                               ]  3.574MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [====>                                              ]  4.197MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=====>                                             ]  5.241MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [====>                                              ]  4.086MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [======>                                            ]   6.29MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=======>                                           ]  7.338MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [====>                                              ]  4.602MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [========>                                          ]  8.383MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=========>                                         ]   9.44MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=====>                                             ]   5.11MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [>                                                  ]  530.8kB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [==========>                                        ]  10.49MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [===========>                                       ]  11.55MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=====>                                             ]   5.63MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [============>                                      ]  12.59MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=============>                                     ]  13.64MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [======>                                            ]  6.151MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [==============>                                    ]   14.7MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [===============>                                   ]  15.75MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [======>                                            ]  6.658MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [>                                                  ]  1.059MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [================>                                  ]   16.8MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=======>                                           ]  7.175MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [=================>                                 ]  17.86MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [==================>                                ]  18.91MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=======>                                           ]  7.695MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [===================>                               ]  19.95MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [====================>                              ]     21MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [========>                                          ]  8.215MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [=====================>                             ]  22.06MB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [>                                                  ]    1.6MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [========>                                          ]  8.723MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [======================>                            ]  23.11MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=======================>                           ]  24.16MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=========>                                         ]  9.235MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [=======================>                           ]  24.68MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [========================>                          ]  25.73MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=========>                                         ]  9.743MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [=========================>                         ]  26.25MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [==========>                                        ]  10.25MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [>                                                  ]  2.128MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [==========================>                        ]   27.3MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [===========================>                       ]  28.35MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [==========>                                        ]  10.76MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [===========================>                       ]  28.87MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [===========>                                       ]  11.27MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [============================>                      ]  29.92MB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [>                                                  ]  2.665MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [===========>                                       ]  11.78MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [=============================>                     ]  30.98MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [============>                                      ]   12.3MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [==============================>                    ]  32.03MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [===============================>                   ]  32.56MB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [>                                                  ]  3.201MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [============>                                      ]  12.82MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [================================>                  ]  33.61MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [================================>                  ]  34.14MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=================================>                 ]  34.66MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=============>                                     ]  13.33MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [==================================>                ]  35.72MB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [>                                                  ]  3.742MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [==================================>                ]  36.24MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=============>                                     ]  13.84MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [===================================>               ]  37.28MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [==============>                                    ]  14.36MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [====================================>              ]  38.33MB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [=>                                                 ]  4.279MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [=====================================>             ]  38.85MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [==============>                                    ]  14.87MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [======================================>            ]   39.9MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [======================================>            ]  40.43MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [===============>                                   ]  15.39MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [========================================>          ]  41.49MB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [=>                                                 ]  4.811MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [===============>                                   ]  15.89MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [=========================================>         ]  42.54MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=========================================>         ]  43.06MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [================>                                  ]   16.4MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [==========================================>        ]  44.11MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [================>                                  ]  16.91MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [=>                                                 ]  5.348MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [===========================================>       ]  45.16MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=================>                                 ]  17.42MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [============================================>      ]  45.68MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [============================================>      ]  46.21MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [=================>                                 ]  17.93MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [=>                                                 ]  5.876MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [=============================================>     ]  47.26MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [==============================================>    ]  47.79MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [==================>                                ]  18.45MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [===============================================>   ]  48.83MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [==================>                                ]  18.97MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [=>                                                 ]  6.409MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Downloading [===============================================>   ]  49.37MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [===================>                               ]  19.47MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [================================================>  ]  50.41MB/51.84MB
[6B[9A[2K
b281ebec60d2: Downloading [===================>                               ]  19.98MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Downloading [=================================================> ]  50.94MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Downloading [=================================================> ]  51.46MB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [=>                                                 ]  6.949MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [====================>                              ]  20.49MB/50.44MB
[9B[6A[2K
e98d6bb51c7c: Verifying Checksum 
[6B[6A[2K
e98d6bb51c7c: Download complete 
[6B[9A[2K
b281ebec60d2: Downloading [====================>                              ]  21.01MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [=====================>                             ]  21.53MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [=>                                                 ]   7.49MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [=====================>                             ]  22.04MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [======================>                            ]  22.55MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [======================>                            ]  23.05MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [==>                                                ]  8.031MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [=======================>                           ]  23.56MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [=======================>                           ]  24.07MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [========================>                          ]  24.58MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [==>                                                ]  8.559MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [=========================>                         ]  25.59MB/50.44MB
[9B[4A[2K
fa245e9d6fa2: Downloading [=======>                                           ]     659B/4.203kB
[4B[4A[2K
fa245e9d6fa2: Downloading [==================================================>]  4.203kB/4.203kB
[4B[4A[2K
fa245e9d6fa2: Download complete 
[4B[5A[2K
517ebafd9747: Downloading [==>                                                ]    9.1MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [=========================>                         ]   26.1MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [==>                                                ]   9.64MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [==========================>                        ]  26.61MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [==========================>                        ]  27.12MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [==>                                                ]  10.18MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [===========================>                       ]  27.63MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [============================>                      ]  28.65MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [==>                                                ]  10.72MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [============================>                      ]  29.17MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [=============================>                     ]  30.19MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [==============================>                    ]  31.21MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [==>                                                ]  11.26MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [===============================>                   ]  31.72MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [>                                                  ]  347.4kB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [================================>                  ]  32.75MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [===>                                               ]  11.79MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=>                                                 ]  1.043MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [=================================>                 ]  33.76MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [=================================>                 ]  34.27MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [==>                                                ]  1.387MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [==================================>                ]  35.29MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [===>                                               ]  12.33MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [==>                                                ]  1.731MB/33.89MB
[3B[3A[2K
662bb10a8d17: Downloading [===>                                               ]  2.075MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [===================================>               ]   36.3MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [===>                                               ]  2.427MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [===>                                               ]  12.87MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [====================================>              ]  37.32MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [====>                                              ]  2.771MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [=====================================>             ]  38.33MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [====>                                              ]  3.124MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [======================================>            ]  38.84MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [===>                                               ]   13.4MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=====>                                             ]  3.468MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [=======================================>           ]  39.86MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [=====>                                             ]  3.812MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [===>                                               ]  13.94MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [========================================>          ]  40.87MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [======>                                            ]  4.164MB/33.89MB
[3B[3A[2K
662bb10a8d17: Downloading [======>                                            ]  4.508MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [=========================================>         ]  41.89MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [===>                                               ]  14.47MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [==========================================>        ]   42.4MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [=======>                                           ]  4.852MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [==========================================>        ]  42.91MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [===>                                               ]  15.01MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=======>                                           ]  5.196MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [===========================================>       ]  43.93MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [========>                                          ]   5.54MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [====>                                              ]  15.54MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [============================================>      ]  44.95MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [========>                                          ]  5.888MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [====>                                              ]  16.08MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [=============================================>     ]  45.96MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [=========>                                         ]  6.241MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [==============================================>    ]  46.98MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [=========>                                         ]  6.585MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [====>                                              ]  16.62MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [===============================================>   ]  47.49MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [==========>                                        ]  6.933MB/33.89MB
[3B[9A[2K
b281ebec60d2: Downloading [===============================================>   ]     48MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [==========>                                        ]  7.285MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [====>                                              ]  17.15MB/192.5MB
[5B[9A[2K
b281ebec60d2: Downloading [================================================>  ]  49.02MB/50.44MB
[9B[9A[2K
b281ebec60d2: Downloading [=================================================> ]  49.52MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [====>                                              ]  17.69MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [===========>                                       ]  7.625MB/33.89MB
[3B[9A[2K
b281ebec60d2: Verifying Checksum 
[9B[9A[2K
b281ebec60d2: Download complete 
[9B[9A[2K
b281ebec60d2: Extracting [>                                                  ]  524.3kB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [====>                                              ]  18.22MB/192.5MB
[5B[9A[2K
b281ebec60d2: Extracting [==========>                                        ]  11.01MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [============>                                      ]  8.326MB/33.89MB
[3B[9A[2K
b281ebec60d2: Extracting [===================>                               ]   19.4MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [====>                                              ]  18.76MB/192.5MB
[5B[9A[2K
b281ebec60d2: Extracting [==========================>                        ]  26.74MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [=============>                                     ]   9.01MB/33.89MB
[3B[9A[2K
b281ebec60d2: Extracting [======================================>            ]   38.8MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [=====>                                             ]   19.3MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=============>                                     ]  9.354MB/33.89MB
[3B[9A[2K
b281ebec60d2: Extracting [=============================================>     ]  46.14MB/50.44MB
[9B[5A[2K
517ebafd9747: Downloading [=====>                                             ]  19.83MB/192.5MB
[5B[9A[2K
b281ebec60d2: Extracting [=================================================> ]  49.81MB/50.44MB
[9B[3A[2K
662bb10a8d17: Downloading [==============>                                    ]  10.04MB/33.89MB
[3B[9A[2K
b281ebec60d2: Extracting [==================================================>]  50.44MB/50.44MB
[9B[9A[2K
b281ebec60d2: Pull complete 
[9B[8A[2K
74dae484504b: Extracting [>                                                  ]   98.3kB/7.856MB
[8B[5A[2K
517ebafd9747: Downloading [=====>                                             ]  20.37MB/192.5MB
[5B[8A[2K
74dae484504b: Extracting [===============================================>   ]  7.471MB/7.856MB
[8B[8A[2K
74dae484504b: Extracting [==================================================>]  7.856MB/7.856MB
[8B[8A[2K
74dae484504b: Extracting [==================================================>]  7.856MB/7.856MB
[8B[3A[2K
662bb10a8d17: Downloading [===============>                                   ]  10.73MB/33.89MB
[3B[8A[2K
74dae484504b: Pull complete 
[8B[7A[2K
21739e3ef21a: Extracting [>                                                  ]  131.1kB/9.997MB
[7B[5A[2K
517ebafd9747: Downloading [=====>                                             ]  20.91MB/192.5MB
[5B[7A[2K
21739e3ef21a: Extracting [==================================================>]  9.997MB/9.997MB
[7B[7A[2K
21739e3ef21a: Pull complete 
[7B[3A[2K
662bb10a8d17: Downloading [================>                                  ]  11.42MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [>                                                  ]  23.93kB/2.279MB
[2B[6A[2K
e98d6bb51c7c: Extracting [>                                                  ]  524.3kB/51.84MB
[6B[5A[2K
517ebafd9747: Downloading [=====>                                             ]  21.45MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Extracting [=============>                                     ]  14.16MB/51.84MB
[6B[2A[2K
fad28b720f14: Downloading [=>                                                 ]  47.05kB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [=================>                                 ]  12.11MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [=====>                                             ]  21.99MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Extracting [====================>                              ]   21.5MB/51.84MB
[6B[2A[2K
fad28b720f14: Downloading [==>                                                ]  122.9kB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [==================>                                ]   12.8MB/33.89MB
[3B[6A[2K
e98d6bb51c7c: Extracting [=========================>                         ]  26.21MB/51.84MB
[6B[2A[2K
fad28b720f14: Downloading [===>                                               ]  171.5kB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [=====>                                             ]  22.52MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Extracting [===============================>                   ]  33.03MB/51.84MB
[6B[2A[2K
fad28b720f14: Downloading [=====>                                             ]  261.4kB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [===================>                               ]  13.49MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [=====>                                             ]  23.06MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Extracting [====================================>              ]  38.27MB/51.84MB
[6B[3A[2K
662bb10a8d17: Downloading [====================>                              ]  13.84MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [======>                                            ]   23.6MB/192.5MB
[5B[2A[2K
fad28b720f14: Downloading [=======>                                           ]  326.9kB/2.279MB
[2B[6A[2K
e98d6bb51c7c: Extracting [=============================================>     ]  46.66MB/51.84MB
[6B[3A[2K
662bb10a8d17: Downloading [=====================>                             ]  14.53MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [======>                                            ]  24.14MB/192.5MB
[5B[6A[2K
e98d6bb51c7c: Extracting [=================================================> ]  50.86MB/51.84MB
[6B[2A[2K
fad28b720f14: Downloading [==========>                                        ]    458kB/2.279MB
[2B[6A[2K
e98d6bb51c7c: Extracting [==================================================>]  51.84MB/51.84MB
[6B[6A[2K
e98d6bb51c7c: Pull complete 
[6B[5A[2K
517ebafd9747: Downloading [======>                                            ]  24.68MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [======================>                            ]  15.22MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [============>                                      ]  556.3kB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [=======================>                           ]  15.91MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [==============>                                    ]  654.6kB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [======>                                            ]  25.76MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=======================>                           ]  16.25MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [===============>                                   ]  720.1kB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [======>                                            ]   26.3MB/192.5MB
[5B[2A[2K
fad28b720f14: Downloading [=================>                                 ]  818.4kB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [========================>                          ]  16.94MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [======>                                            ]  26.84MB/192.5MB
[5B[2A[2K
fad28b720f14: Downloading [===================>                               ]    884kB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [=======>                                           ]  27.38MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [==========================>                        ]  17.64MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [======================>                            ]  1.011MB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [==========================>                        ]  17.98MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [=======>                                           ]  27.92MB/192.5MB
[5B[2A[2K
fad28b720f14: Downloading [========================>                          ]  1.109MB/2.279MB
[2B[2A[2K
fad28b720f14: Downloading [=========================>                         ]  1.175MB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [=======>                                           ]  28.45MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [===========================>                       ]  18.67MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [===========================>                       ]  1.273MB/2.279MB
[2B[2A[2K
fad28b720f14: Downloading [==============================>                    ]  1.404MB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [=============================>                     ]   19.7MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [=================================>                 ]  1.535MB/2.279MB
[2B[3A[2K
662bb10a8d17: Downloading [==============================>                    ]  20.38MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [====================================>              ]  1.666MB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [=======>                                           ]  29.53MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [===============================>                   ]  21.07MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [=====================================>             ]  1.732MB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [=======>                                           ]  30.07MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [===============================>                   ]  21.42MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [=========================================>         ]  1.896MB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [=======>                                           ]  30.61MB/192.5MB
[5B[2A[2K
fad28b720f14: Downloading [============================================>      ]   2.03MB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [========>                                          ]  31.15MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=================================>                 ]  22.45MB/33.89MB
[3B[3A[2K
662bb10a8d17: Downloading [=================================>                 ]   22.8MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [==============================================>    ]  2.128MB/2.279MB
[2B[5A[2K
517ebafd9747: Downloading [========>                                          ]  31.69MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [==================================>                ]  23.14MB/33.89MB
[3B[2A[2K
fad28b720f14: Downloading [=================================================> ]  2.259MB/2.279MB
[2B[2A[2K
fad28b720f14: Verifying Checksum 
[2B[2A[2K
fad28b720f14: Download complete 
[2B[5A[2K
517ebafd9747: Downloading [========>                                          ]  32.76MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [===================================>               ]  24.18MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [========>                                          ]   33.3MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [====================================>              ]  24.87MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [========>                                          ]  34.38MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=====================================>             ]  25.55MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [=========>                                         ]  35.46MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [======================================>            ]  26.24MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [=========>                                         ]  36.54MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=======================================>           ]  26.93MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [=========>                                         ]  37.61MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [========================================>          ]  27.27MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [==========>                                        ]  38.69MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=========================================>         ]  27.96MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [==========>                                        ]  39.23MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=========================================>         ]   28.3MB/33.89MB
[3B[3A[2K
662bb10a8d17: Downloading [==========================================>        ]  28.65MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [==========>                                        ]  40.31MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [===========================================>       ]  29.33MB/33.89MB
[3B[3A[2K
662bb10a8d17: Downloading [===========================================>       ]  29.69MB/33.89MB
[3B[1A[2K
512c94f3667e: Downloading [==================================================>]     451B/451B
[1B[1A[2K
512c94f3667e: Download complete 
[1B[5A[2K
517ebafd9747: Downloading [==========>                                        ]  41.39MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==========>                                        ]  41.92MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [============================================>      ]  30.04MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [===========>                                       ]  42.46MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=============================================>     ]  31.08MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [===========>                                       ]  44.08MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [==============================================>    ]  31.42MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [===========>                                       ]  45.16MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [==============================================>    ]  31.77MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [===========>                                       ]  45.71MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============>                                      ]  46.25MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [===============================================>   ]  32.47MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [============>                                      ]  47.32MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [================================================>  ]  32.81MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [============>                                      ]   48.4MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=================================================> ]   33.5MB/33.89MB
[3B[5A[2K
517ebafd9747: Downloading [============>                                      ]  49.48MB/192.5MB
[5B[3A[2K
662bb10a8d17: Downloading [=================================================> ]  33.84MB/33.89MB
[3B[3A[2K
662bb10a8d17: Verifying Checksum 
[3B[3A[2K
662bb10a8d17: Download complete 
[3B[5A[2K
517ebafd9747: Downloading [=============>                                     ]  50.56MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============>                                     ]  51.64MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============>                                     ]  52.72MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============>                                     ]  53.79MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============>                                    ]  54.86MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============>                                    ]  55.94MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============>                                    ]  57.01MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============>                                   ]  58.09MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============>                                   ]  59.16MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============>                                   ]  60.24MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============>                                   ]  61.32MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================>                                  ]   62.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================>                                  ]  63.48MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================>                                  ]  64.55MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================>                                 ]  65.61MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================>                                 ]  67.22MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================>                                 ]  68.29MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================>                                 ]  68.83MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==================>                                ]  69.91MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==================>                                ]  70.99MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==================>                                ]  72.06MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===================>                               ]  73.67MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===================>                               ]  74.21MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===================>                               ]  75.29MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===================>                               ]   76.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [====================>                              ]  77.97MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [====================>                              ]  79.59MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=====================>                             ]   81.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=====================>                             ]  82.27MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=====================>                             ]  83.34MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=====================>                             ]  84.43MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [======================>                            ]   85.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [======================>                            ]   87.1MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================>                           ]  88.72MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================>                           ]  89.78MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================>                           ]  90.86MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================>                           ]   91.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [========================>                          ]  92.46MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [========================>                          ]  94.08MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [========================>                          ]  95.16MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=========================>                         ]  96.78MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=========================>                         ]  97.31MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=========================>                         ]  98.39MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=========================>                         ]    100MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==========================>                        ]  100.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==========================>                        ]  101.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==========================>                        ]  103.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================>                       ]  104.3MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================>                       ]  104.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================>                       ]  105.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================>                       ]    107MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================>                       ]  107.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============================>                      ]  108.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============================>                      ]  109.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============================>                      ]  110.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================>                     ]  111.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================>                     ]  112.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================>                     ]    114MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================>                     ]  115.1MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============================>                    ]  116.1MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============================>                    ]  117.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============================>                    ]  118.3MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============================>                   ]  119.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============================>                   ]  120.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============================>                   ]  121.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============================>                   ]  122.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================================>                  ]  123.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================================>                  ]  124.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================================>                  ]  125.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================================>                  ]  126.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================================>                 ]  127.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================================>                 ]  128.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================================>                 ]  129.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================================>                 ]  130.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==================================>                ]  131.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==================================>                ]  132.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==================================>                ]  133.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==================================>                ]  134.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===================================>               ]  136.1MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===================================>               ]  137.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [====================================>              ]  138.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [====================================>              ]  139.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [====================================>              ]  141.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [====================================>              ]    142MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=====================================>             ]  143.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=====================================>             ]  144.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=====================================>             ]  145.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [======================================>            ]  146.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [======================================>            ]  147.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [======================================>            ]  149.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================================>           ]  150.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================================>           ]  151.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================================>           ]  152.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=======================================>           ]  153.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [========================================>          ]  155.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [========================================>          ]  156.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [========================================>          ]  157.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=========================================>         ]  158.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=========================================>         ]  159.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=========================================>         ]  161.3MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==========================================>        ]  162.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==========================================>        ]    164MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================================>       ]  165.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================================>       ]  166.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================================>       ]  167.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===========================================>       ]  168.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============================================>      ]  169.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============================================>      ]    171MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============================================>      ]  172.1MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [============================================>      ]  173.1MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================================>     ]  174.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================================>     ]  175.3MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================================>     ]  175.8MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=============================================>     ]  176.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============================================>    ]  178.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============================================>    ]  179.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [==============================================>    ]  180.7MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============================================>   ]  182.3MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [===============================================>   ]  183.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================================================>  ]  185.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================================================>  ]  187.1MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [================================================>  ]  188.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================================================> ]  189.3MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================================================> ]  190.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Downloading [=================================================> ]  191.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Verifying Checksum 
[5B[5A[2K
517ebafd9747: Download complete 
[5B[5A[2K
517ebafd9747: Extracting [>                                                  ]  557.1kB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [==>                                                ]  10.03MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [===>                                               ]  12.26MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [===>                                               ]  15.04MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [====>                                              ]  17.83MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [========>                                          ]   31.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [===========>                                       ]  42.89MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [==============>                                    ]  56.26MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [================>                                  ]  61.83MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [=================>                                 ]  66.85MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [===================>                               ]  76.87MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [======================>                            ]   86.9MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [=========================>                         ]  98.04MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [=============================>                     ]    112MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [===============================>                   ]  122.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [==================================>                ]  132.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [====================================>              ]  140.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [=======================================>           ]  150.4MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [===========================================>       ]  166.6MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [==============================================>    ]  178.3MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [================================================>  ]  185.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [=================================================> ]  190.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [=================================================> ]  192.2MB/192.5MB
[5B[5A[2K
517ebafd9747: Extracting [==================================================>]  192.5MB/192.5MB
[5B[5A[2K
517ebafd9747: Pull complete 
[5B[4A[2K
fa245e9d6fa2: Extracting [==================================================>]  4.203kB/4.203kB
[4B[4A[2K
fa245e9d6fa2: Extracting [==================================================>]  4.203kB/4.203kB
[4B[4A[2K
fa245e9d6fa2: Pull complete 
[4B[3A[2K
662bb10a8d17: Extracting [>                                                  ]  360.4kB/33.89MB
[3B[3A[2K
662bb10a8d17: Extracting [===================>                               ]  12.98MB/33.89MB
[3B[3A[2K
662bb10a8d17: Extracting [=======================================>           ]  26.67MB/33.89MB
[3B[3A[2K
662bb10a8d17: Extracting [===============================================>   ]  32.08MB/33.89MB
[3B[3A[2K
662bb10a8d17: Extracting [==================================================>]  33.89MB/33.89MB
[3B[3A[2K
662bb10a8d17: Pull complete 
[3B[2A[2K
fad28b720f14: Extracting [>                                                  ]  32.77kB/2.279MB
[2B[2A[2K
fad28b720f14: Extracting [==================================================>]  2.279MB/2.279MB
[2B[2A[2K
fad28b720f14: Pull complete 
[2B[1A[2K
512c94f3667e: Extracting [==================================================>]     451B/451B
[1B[1A[2K
512c94f3667e: Extracting [==================================================>]     451B/451B
[1B[1A[2K
512c94f3667e: Pull complete 
[1BDigest: sha256:ffe804d6fcced29bcfc3477de079d03a9c2b0e4917e44bfeafb1a6b0f875e383
Status: Downloaded newer image for node:lts
 ---> 424bc28f998d
Step 2/7 : RUN mkdir -p /opt/app
 ---> Running in 69e15168c58e
Removing intermediate container 69e15168c58e
 ---> e84212aa932f
Step 3/7 : RUN git clone https://github.com/DHFinance/dhf-pay-processor.git /opt/app/casper-processor
 ---> Running in 6534463b690f
[91mCloning into '/opt/app/casper-processor'...
[0mRemoving intermediate container 6534463b690f
 ---> 77f99cb7d789
Step 4/7 : WORKDIR /opt/app/casper-processor
 ---> Running in 4752fb5868fc
Removing intermediate container 4752fb5868fc
 ---> 583959de89f1
Step 5/7 : COPY .env /opt/app/casper-processor/.env
 ---> f497e8a007fb
Step 6/7 : RUN npm i
 ---> Running in 8f7bf34e9164
[91mnpm[0m[91m WARN[0m[91m old lockfile 
npm WARN[0m[91m old lockfile The package-lock.json file was created with an old version of npm,
npm WARN[0m[91m [0m[91mold lockfile so supplemental metadata must be fetched from the registry.
npm WARN old lockfile[0m[91m 
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile 
[0m[91mnpm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
[0m[91mnpm WARN deprecated formidable@1.2.6: Please upgrade to latest, formidable@v2 or formidable@v3! Check these notes: https://bit.ly/2ZEqIau
[0m[91mnpm WARN deprecated har-validator@5.1.5: this library is no longer supported
[0m[91mnpm WARN deprecated uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
[0m[91mnpm WARN deprecated node-pre-gyp@0.11.0: Please upgrade to @mapbox/node-pre-gyp: the non-scoped node-pre-gyp package is deprecated and only the @mapbox scoped package will recieve updates in the future
[0m[91mnpm WARN deprecated superagent@5.3.1: Please upgrade to v7.0.2+ of superagent.  We have fixed numerous issues with streams, form-data, attach(), filesystem errors not bubbling up (ENOENT on attach()), and all tests are now passing.  See the releases tab for more information at <https://github.com/visionmedia/superagent/releases>.
[0m[91mnpm WARN deprecated tar@2.2.2: This version of tar is no longer supported, and will not receive security updates. Please upgrade asap.
[0m[91mnpm WARN deprecated core-js@2.6.12: core-js@<3.4 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Please, upgrade your dependencies to the actual version of core-js.
[0m
added 1197 packages, and audited 1455 packages in 41s

96 packages are looking for funding
  run `npm fund` for details

25 vulnerabilities (9 moderate, 13 high, 3 critical)

To address issues that do not require attention, run:
  npm audit fix

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[91mnpm notice 
npm notice New minor version of npm available! 8.5.0 -> 8.7.0
npm notice Changelog: <https://github.com/npm/cli/releases/tag/v8.7.0>
[0m[91mnpm notice[0m[91m Run `npm install -g npm@8.7.0` to update!
npm notice 
[0mRemoving intermediate container 8f7bf34e9164
 ---> 7b12db1503e8
Step 7/7 : RUN npm run build
 ---> Running in f4078aee5618

> blockchain@0.0.1 prebuild
> rimraf dist


> blockchain@0.0.1 build
> nest build

Removing intermediate container f4078aee5618
 ---> 80122ef2f2d5
Successfully built 80122ef2f2d5
Successfully tagged dhf-pay-deploy_casper-processor:latest
Sending build context to Docker daemon     611B

Step 1/10 : FROM node:lts
 ---> 424bc28f998d
Step 2/10 : RUN mkdir -p /opt/app
 ---> Using cache
 ---> e84212aa932f
Step 3/10 : RUN git clone https://github.com/DHFinance/dhf-pay-back.git /opt/app/casper-back
 ---> Running in 105f5f177050
[91mCloning into '/opt/app/casper-back'...
[0mRemoving intermediate container 105f5f177050
 ---> 75206ef984d4
Step 4/10 : WORKDIR /opt/app/casper-back
 ---> Running in 2ef7bcef3096
Removing intermediate container 2ef7bcef3096
 ---> 598614da8ee8
Step 5/10 : COPY .env /opt/app/casper-back/.env
 ---> 21120b5a3a84
Step 6/10 : RUN  npm install -g npm@8.3.0
 ---> Running in 4851a9789ee8

removed 4 packages, changed 47 packages, and audited 215 packages in 11s

10 packages are looking for funding
  run `npm fund` for details

1 moderate severity vulnerability

To address all issues, run:
  npm audit fix

Run `npm audit` for details.
[91mnpm notice[0m[91m 
npm notice New minor version of npm available! 8.5.0 -> 8.7.0
npm [0m[91mnotice Changelog: <https://github.com/npm/cli/releases/tag/v8.7.0>
npm[0m[91m notice Run `npm install -g npm@8.7.0` to update!
npm notice 
[0mRemoving intermediate container 4851a9789ee8
 ---> a585005e9be0
Step 7/10 : RUN npm install node-pre-gyp -g
 ---> Running in 2651ecf76ffd
[91mnpm WARN deprecated node-pre-gyp@0.17.0: Please upgrade to @mapbox/node-pre-gyp: the non-scoped node-pre-gyp package is deprecated and only the @mapbox scoped package will recieve updates in the future
[0m
added 67 packages, and audited 68 packages in 4s

2 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
Removing intermediate container 2651ecf76ffd
 ---> 150000d84f73
Step 8/10 : RUN npm i
 ---> Running in 7f92f24bd9f9
[91mnpm[0m[91m WARN old lockfile 
npm WARN[0m[91m old lockfile The package-lock.json file was created with an old version of npm,
[0m[91mnpm WARN old lockfile so supplemental metadata must be fetched from the registry.
npm [0m[91mWARN [0m[91mold lockfile 
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile 
[0m[91mnpm WARN deprecated superagent@7.1.2: Deprecated due to bug in CI build https://github.com/visionmedia/superagent/pull/1677\#issuecomment-1081361876
[0m[91mnpm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
[0m[91mnpm WARN deprecated node-pre-gyp@0.11.0: Please upgrade to @mapbox/node-pre-gyp: the non-scoped node-pre-gyp package is deprecated and only the @mapbox scoped package will recieve updates in the future
[0m[91mnpm WARN deprecated har-validator@5.1.5: this library is no longer supported
[0m[91mnpm WARN deprecated uuid@3.4.0: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
[0m[91mnpm WARN deprecated tar@2.2.2: This version of tar is no longer supported, and will not receive security updates. Please upgrade asap.
[0m
added 1128 packages, and audited 1386 packages in 33s

108 packages are looking for funding
  run `npm fund` for details

20 vulnerabilities (10 moderate, 7 high, 3 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
Removing intermediate container 7f92f24bd9f9
 ---> 7a1d4e4ff724
Step 9/10 : Run npm install --save-dev webpack
 ---> Running in c1bfcc63e813

added 7 packages, and audited 1393 packages in 1s

109 packages are looking for funding
  run `npm fund` for details

20 vulnerabilities (10 moderate, 7 high, 3 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
Removing intermediate container c1bfcc63e813
 ---> 99cbe1121943
Step 10/10 : RUN npm run build
 ---> Running in c2b78bbefdc1

> blockchain@0.0.1 prebuild
> rimraf dist


> blockchain@0.0.1 build
> nest build

Removing intermediate container c2b78bbefdc1
 ---> 293666f29bcd
Successfully built 293666f29bcd
Successfully tagged dhf-pay-deploy_casper-back:latest
Sending build context to Docker daemon     433B

Step 1/8 : FROM node:lts
 ---> 424bc28f998d
Step 2/8 : RUN mkdir -p /opt/app
 ---> Using cache
 ---> e84212aa932f
Step 3/8 : RUN  git clone https://github.com/DHFinance/dhf-pay-front.git /opt/app/casper-front
 ---> Running in f2cd47f2f47c
[91mCloning into '/opt/app/casper-front'...
[0mRemoving intermediate container f2cd47f2f47c
 ---> 2c87f6340919
Step 4/8 : WORKDIR /opt/app/casper-front
 ---> Running in cd8780129de7
Removing intermediate container cd8780129de7
 ---> 31aecacb7d35
Step 5/8 : COPY .env.server /opt/app/casper-front/.env
 ---> 12565e9f2b16
Step 6/8 : RUN  npm install -g npm@8.3.0
 ---> Running in 4528410c1d25

removed 4 packages, changed 47 packages, and audited 215 packages in 10s

10 packages are looking for funding
  run `npm fund` for details

1 moderate severity vulnerability

To address all issues, run:
  npm audit fix

Run `npm audit` for details.
[91mnpm notice[0m[91m 
npm notice New minor version of npm available! 8.5.0 -> 8.7.0
npm [0m[91mnotice Changelog: <https://github.com/npm/cli/releases/tag/v8.7.0>
npm notice Run `npm install -g npm@8.7.0` to update!
npm[0m[91m notice 
[0mRemoving intermediate container 4528410c1d25
 ---> 07370345df0e
Step 7/8 : RUN npm i
 ---> Running in f1ac3d532153
[91mnpm[0m[91m WARN old lockfile 
npm WARN old lockfile The package-lock.json file was created with an old version of npm,
[0m[91mnpm WARN [0m[91mold lockfile so supplemental metadata must be fetched from the registry.
npm WARN [0m[91mold lockfile 
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile 
[0m[91mnpm WARN deprecated source-map-resolve@0.6.0: See https://github.com/lydell/source-map-resolve#deprecated
[0m[91mnpm WARN deprecated redux-devtools-extension@2.13.9: Package moved to @redux-devtools/extension.
[0m[91mnpm WARN deprecated querystring@0.2.1: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
[0m[91mnpm WARN deprecated @zeit/next-css@1.0.1: Next.js now has built-in support for CSS: https://nextjs.org/docs/basic-features/built-in-css-support. The built-in support solves many bugs and painpoints that the next-css plugin had.
[0m
added 1037 packages, and audited 1295 packages in 40s

112 packages are looking for funding
  run `npm fund` for details

13 vulnerabilities (11 moderate, 1 high, 1 critical)

To address issues that do not require attention, run:
  npm audit fix

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
Removing intermediate container f1ac3d532153
 ---> 3e410e90da9f
Step 8/8 : RUN npm run build
 ---> Running in 9f6cca7aa988

> build
> next build

info  - Loaded env from /opt/app/casper-front/.env
Attention: Next.js now collects completely anonymous telemetry regarding usage.
This information is used to shape Next.js' roadmap and prioritize features.
You can learn more, including how to opt-out if you'd not like to participate in this anonymous program, by visiting the following URL:
https://nextjs.org/telemetry

info  - Checking validity of types...

./src/components/Forms/Bill/index.tsx
158:8  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps
170:8  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/InvoicesBuilder/index.tsx
46:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
56:8  Warning: React Hook useEffect has missing dependencies: 'activeStores', 'dispatch', and 'user.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/Login/index.tsx
58:8  Warning: React Hook useEffect has missing dependencies: 'form', 'userData.email', and 'userData.password'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/PaymentsButton/index.tsx
47:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/Register/index.tsx
74:8  Warning: React Hook useEffect has a missing dependency: 'form'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps
213:8  Warning: React Hook useEffect has missing dependencies: 'fieldError' and 'form'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Forms/Restore/index.tsx
79:8  Warning: React Hook useEffect has a missing dependency: 'form'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps
170:8  Warning: React Hook useEffect has missing dependencies: 'fieldError' and 'form'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/Payment/index.tsx
74:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
81:8  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/Store/index.tsx
77:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/Transaction/index.tsx
57:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Info/User/index.tsx
32:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'router.query.slug'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Paymets/index.tsx
53:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
70:8  Warning: React Hook useEffect has missing dependencies: 'activeStores', 'dispatch', and 'user.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
76:8  Warning: React Hook useEffect has a missing dependency: 'currentStore'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Stores/index.tsx
89:8  Warning: React Hook useEffect has missing dependencies: 'dispatch' and 'user.id'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Transactions/index.tsx
59:8  Warning: React Hook useEffect has missing dependencies: 'dispatch', 'user.id', and 'user?.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps
65:8  Warning: React Hook useEffect has missing dependencies: 'activeStores', 'dispatch', and 'user.role'. Either include them or remove the dependency array.  react-hooks/exhaustive-deps

./src/components/Tables/Users/index.tsx
42:8  Warning: React Hook useEffect has a missing dependency: 'dispatch'. Either include it or remove the dependency array.  react-hooks/exhaustive-deps

info  - Need to disable some ESLint rules? Learn more here: https://nextjs.org/docs/basic-features/eslint#disabling-rules
info  - Creating an optimized production build...
info  - Disabled SWC as replacement for Babel because of custom Babel configuration ".babelrc" https://nextjs.org/docs/messages/swc-disabled
info  - Using external babel configuration from /opt/app/casper-front/.babelrc
[91m(node:20) [DEP_WEBPACK_MODULE_UPDATE_HASH] DeprecationWarning: Module.updateHash: Use new ChunkGraph API
(Use `node --trace-deprecation ...` to show where the warning was created)
[0minfo  - Compiled successfully
info  - Collecting page data...
info  - Generating static pages (0/19)
info  - Generating static pages (4/19)
info  - Generating static pages (9/19)
info  - Generating static pages (14/19)
info  - Generating static pages (19/19)
info  - Finalizing page optimization...

Page                                       Size     First Load JS
┌ ○ / (912 ms)                             1.63 kB         202 kB
├   /_app                                  0 B            98.9 kB
├ ○ /404                                   2.85 kB         102 kB
├ λ /api/hello                             0 B            98.9 kB
├ ○ /bill/[slug]                           54.7 kB         483 kB
├ ○ /buttons (922 ms)                      2.72 kB         278 kB
├ ○ /buttons/[slug] (943 ms)               401 B           245 kB
├ ○ /buttonsBuilder (949 ms)               3.89 kB         249 kB
├ ○ /invoices (958 ms)                     2.71 kB         278 kB
├ ○ /invoices/[slug] (908 ms)              397 B           245 kB
├ ○ /invoicesBuilder (949 ms)              3.04 kB         248 kB
├ ○ /login (943 ms)                        2.93 kB         224 kB
├ ○ /register (470 ms)                     2.89 kB         224 kB
├ ○ /restore (932 ms)                      2.93 kB         224 kB
├ ○ /stores (594 ms)                       3.16 kB         520 kB
├ ○ /stores/[slug]                         5.24 kB         464 kB
├ ○ /transactions (937 ms)                 2.14 kB         277 kB
├ ○ /transactions/[slug]                   3.08 kB         433 kB
├ ○ /users (915 ms)                        1.79 kB         277 kB
└ ○ /users/[slug] (911 ms)                 3.02 kB         213 kB
+ First Load JS shared by all              98.9 kB
  ├ chunks/framework-bb5c596eafb42b22.js   42.1 kB
  ├ chunks/main-8a0fe121e379d1aa.js        29.9 kB
  ├ chunks/pages/_app-62f3ad37d9f17071.js  25.3 kB
  ├ chunks/webpack-fa1c5fe73b1a0886.js     1.6 kB
  └ css/b3ff8ad54ff5b445.css               272 B

λ  (Server)  server-side renders at runtime (uses getInitialProps or getServerSideProps)
○  (Static)  automatically rendered as static HTML (uses no initial props)

Removing intermediate container 9f6cca7aa988
 ---> 15b0ed6cd6ff
Successfully built 15b0ed6cd6ff
Successfully tagged dhf-pay-deploy_casper-front:latest
Attaching to casper-back, casper-db, casper-front, casper-processor, casper-rabbitmq
casper-db         | The files belonging to this database system will be owned by user "postgres".
casper-db         | This user must also own the server process.
casper-db         | 
casper-db         | The database cluster will be initialized with locale "en_US.utf8".
casper-db         | The default database encoding has accordingly been set to "UTF8".
casper-db         | The default text search configuration will be set to "english".
casper-db         | 
casper-db         | Data page checksums are disabled.
casper-db         | 
casper-db         | fixing permissions on existing directory /var/lib/postgresql/data ... ok
casper-db         | creating subdirectories ... ok
casper-db         | selecting dynamic shared memory implementation ... posix
casper-db         | selecting default max_connections ... 100
casper-db         | selecting default shared_buffers ... 128MB
casper-db         | selecting default time zone ... Etc/UTC
casper-db         | creating configuration files ... ok
casper-db         | running bootstrap script ... ok
casper-front      | 
casper-front      | > start
casper-front      | > next start
casper-front      | 
casper-front      | ready - started server on 0.0.0.0:3000, url: http://localhost:3000
casper-front      | info  - Loaded env from /opt/app/casper-front/.env
casper-processor  | 
casper-processor  | > blockchain@0.0.1 start
casper-processor  | > nest start
casper-processor  | 
casper-db         | performing post-bootstrap initialization ... ok
casper-back       | 
casper-back       | > blockchain@0.0.1 start
casper-back       | > nest start
casper-back       | 
casper-db         | syncing data to disk ... ok
casper-db         | 
casper-db         | 
casper-db         | Success. You can now start the database server using:
casper-db         | 
casper-db         |     pg_ctl -D /var/lib/postgresql/data -l logfile start
casper-db         | 
casper-db         | initdb: warning: enabling "trust" authentication for local connections
casper-db         | You can change this by editing pg_hba.conf or using the option -A, or
casper-db         | --auth-local and --auth-host, the next time you run initdb.
casper-db         | waiting for server to start....2022-04-16 20:37:18.019 UTC [48] LOG:  starting PostgreSQL 14.2 (Debian 14.2-1.pgdg110+1) on x86_64-pc-linux-gnu, compiled by gcc (Debian 10.2.1-6) 10.2.1 20210110, 64-bit
casper-db         | 2022-04-16 20:37:18.023 UTC [48] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
casper-db         | 2022-04-16 20:37:18.034 UTC [49] LOG:  database system was shut down at 2022-04-16 20:37:17 UTC
casper-db         | 2022-04-16 20:37:18.041 UTC [48] LOG:  database system is ready to accept connections
casper-db         |  done
casper-db         | server started
casper-db         | CREATE DATABASE
casper-db         | 
casper-db         | 
casper-db         | /usr/local/bin/docker-entrypoint.sh: ignoring /docker-entrypoint-initdb.d/*
casper-db         | 
casper-db         | 2022-04-16 20:37:18.360 UTC [48] LOG:  received fast shutdown request
casper-db         | waiting for server to shut down....2022-04-16 20:37:18.364 UTC [48] LOG:  aborting any active transactions
casper-db         | 2022-04-16 20:37:18.365 UTC [48] LOG:  background worker "logical replication launcher" (PID 55) exited with exit code 1
casper-db         | 2022-04-16 20:37:18.365 UTC [50] LOG:  shutting down
casper-db         | 2022-04-16 20:37:18.391 UTC [48] LOG:  database system is shut down
casper-db         |  done
casper-db         | server stopped
casper-db         | 
casper-db         | PostgreSQL init process complete; ready for start up.
casper-db         | 
casper-db         | 2022-04-16 20:37:18.477 UTC [1] LOG:  starting PostgreSQL 14.2 (Debian 14.2-1.pgdg110+1) on x86_64-pc-linux-gnu, compiled by gcc (Debian 10.2.1-6) 10.2.1 20210110, 64-bit
casper-db         | 2022-04-16 20:37:18.478 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
casper-db         | 2022-04-16 20:37:18.478 UTC [1] LOG:  listening on IPv6 address "::", port 5432
casper-db         | 2022-04-16 20:37:18.486 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
casper-db         | 2022-04-16 20:37:18.495 UTC [62] LOG:  database system was shut down at 2022-04-16 20:37:18 UTC
casper-db         | 2022-04-16 20:37:18.501 UTC [1] LOG:  database system is ready to accept connections
casper-rabbitmq   | 
casper-rabbitmq   |               RabbitMQ 3.6.16. Copyright (C) 2007-2018 Pivotal Software, Inc.
casper-rabbitmq   |   ##  ##      Licensed under the MPL.  See http://www.rabbitmq.com/
casper-rabbitmq   |   ##  ##
casper-rabbitmq   |   ##########  Logs: tty
casper-rabbitmq   |   ######  ##        tty
casper-rabbitmq   |   ##########
casper-rabbitmq   |               Starting broker...
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:18 ===
casper-rabbitmq   | Starting RabbitMQ 3.6.16 on Erlang 20.3.4
casper-rabbitmq   | Copyright (C) 2007-2018 Pivotal Software, Inc.
casper-rabbitmq   | Licensed under the MPL.  See http://www.rabbitmq.com/
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:18 ===
casper-rabbitmq   | node           : rabbit@5278bcdae952
casper-rabbitmq   | home dir       : /var/lib/rabbitmq
casper-rabbitmq   | config file(s) : /etc/rabbitmq/rabbitmq.config
casper-rabbitmq   | cookie hash    : nhVV5wMpEME4dAGoghvIHA==
casper-rabbitmq   | log            : tty
casper-rabbitmq   | sasl log       : tty
casper-rabbitmq   | database dir   : /var/lib/rabbitmq/mnesia/rabbit@5278bcdae952
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:19 ===
casper-rabbitmq   | Memory high watermark set to 20540 MiB (21537941094 bytes) of 51350 MiB (53844852736 bytes) total
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:19 ===
casper-rabbitmq   | Enabling free disk space monitoring
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:19 ===
casper-rabbitmq   | Disk free limit set to 50MB
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:19 ===
casper-rabbitmq   | Limiting to approx 924 file handles (829 sockets)
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:19 ===
casper-rabbitmq   | FHC read buffering:  OFF
casper-rabbitmq   | FHC write buffering: ON
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:19 ===
casper-rabbitmq   | Database directory at /var/lib/rabbitmq/mnesia/rabbit@5278bcdae952 is empty. Initialising from scratch...
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:19 ===
casper-rabbitmq   |     application: mnesia
casper-rabbitmq   |     exited: stopped
casper-rabbitmq   |     type: temporary
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Waiting for Mnesia tables for 30000 ms, 9 retries left
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Waiting for Mnesia tables for 30000 ms, 9 retries left
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Waiting for Mnesia tables for 30000 ms, 9 retries left
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Priority queues enabled, real BQ is rabbit_variable_queue
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Starting rabbit_node_monitor
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Management plugin: using rates mode 'basic'
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | msg_store_transient: using rabbit_msg_store_ets_index to provide index
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | msg_store_persistent: using rabbit_msg_store_ets_index to provide index
casper-rabbitmq   | 
casper-rabbitmq   | =WARNING REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | msg_store_persistent: rebuilding indices from scratch
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Adding vhost '/'
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Creating user 'guest'
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Setting user tags for user 'guest' to [administrator]
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Setting permissions for 'guest' in '/' to '.*', '.*', '.*'
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | started TCP Listener on [::]:5672
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Management plugin started. Port: 15672
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Statistics database started.
casper-rabbitmq   |  completed with 6 plugins.
casper-rabbitmq   | 
casper-rabbitmq   | =INFO REPORT==== 16-Apr-2022::20:37:20 ===
casper-rabbitmq   | Server startup complete; 6 plugins started.
casper-rabbitmq   |  * rabbitmq_management
casper-rabbitmq   |  * rabbitmq_web_dispatch
casper-rabbitmq   |  * cowboy
casper-rabbitmq   |  * rabbitmq_management_agent
casper-rabbitmq   |  * amqp_client
casper-rabbitmq   |  * cowlib
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[NestFactory] [39m[32mStarting Nest application...[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +33ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mMailerModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mMailerModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mMailerCoreModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mHttpModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mDiscoveryModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mAppModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mScheduleModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mConfigModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-processor  | query: SELECT * FROM current_schema()
casper-processor  | query: SHOW server_version;
casper-processor  | query: START TRANSACTION
casper-processor  | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'typeorm_metadata'
casper-processor  | query: CREATE TABLE "typeorm_metadata" ("type" character varying NOT NULL, "database" character varying, "schema" character varying, "table" character varying, "name" character varying, "value" text)
casper-processor  | query: SELECT * FROM current_schema()
casper-processor  | query: SELECT * FROM current_database()
casper-processor  | query: SELECT "table_schema", "table_name" FROM "information_schema"."tables" WHERE ("table_schema" = 'public' AND "table_name" = 'user') OR ("table_schema" = 'public' AND "table_name" = 'transaction') OR ("table_schema" = 'public' AND "table_name" = 'stores') OR ("table_schema" = 'public' AND "table_name" = 'payment')
casper-processor  | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'typeorm_metadata'
casper-processor  | query: SELECT * FROM current_database()
casper-processor  | query: SELECT * FROM current_schema()
casper-processor  | query: SELECT "t".* FROM "typeorm_metadata" "t" INNER JOIN "pg_catalog"."pg_class" "c" ON "c"."relname" = "t"."name" INNER JOIN "pg_namespace" "n" ON "n"."oid" = "c"."relnamespace" AND "n"."nspname" = "t"."schema" WHERE "t"."type" IN ('VIEW', 'MATERIALIZED_VIEW') AND (1=1)
casper-processor  | query: CREATE TABLE "user" ("id" SERIAL NOT NULL, "name" character varying NOT NULL, "lastName" character varying NOT NULL, "password" character varying NOT NULL, "restorePasswordCode" integer, "emailVerification" integer, "email" character varying NOT NULL, "role" character varying NOT NULL, "company" character varying NOT NULL, "token" character varying NOT NULL, "blocked" boolean NOT NULL, CONSTRAINT "PK_cace4a159ff9f2512dd42373760" PRIMARY KEY ("id"))
casper-processor  | query: CREATE TABLE "transaction" ("id" SERIAL NOT NULL, "status" character varying NOT NULL, "email" character varying NOT NULL, "updated" TIMESTAMP NOT NULL, "txHash" character varying NOT NULL, "sender" character varying NOT NULL, "amount" bigint NOT NULL, "paymentId" integer, CONSTRAINT "PK_89eadb93a89810556e1cbcd6ab9" PRIMARY KEY ("id"))
casper-processor  | query: CREATE TABLE "stores" ("id" SERIAL NOT NULL, "url" character varying NOT NULL, "name" character varying NOT NULL, "wallet" character varying NOT NULL, "description" character varying, "apiKey" character varying, "blocked" boolean NOT NULL, "userId" integer NOT NULL, CONSTRAINT "PK_7aa6e7d71fa7acdd7ca43d7c9cb" PRIMARY KEY ("id"))
casper-processor  | query: CREATE TABLE "payment" ("id" SERIAL NOT NULL, "datetime" TIMESTAMP NOT NULL, "amount" bigint NOT NULL, "status" character varying NOT NULL, "comment" character varying NOT NULL, "type" integer, "text" character varying, "storeId" integer, CONSTRAINT "PK_fcaec7df5adf9cac408c686b2ab" PRIMARY KEY ("id"))
casper-processor  | query: ALTER TABLE "transaction" ADD CONSTRAINT "FK_26ba3b75368b99964d6dea5cc2c" FOREIGN KEY ("paymentId") REFERENCES "payment"("id") ON DELETE NO ACTION ON UPDATE NO ACTION
casper-processor  | query: ALTER TABLE "stores" ADD CONSTRAINT "FK_f36d697e265ed99b80cae6984c9" FOREIGN KEY ("userId") REFERENCES "user"("id") ON DELETE NO ACTION ON UPDATE NO ACTION
casper-processor  | query: ALTER TABLE "payment" ADD CONSTRAINT "FK_3a767f0d31e2535c8edfc2d3667" FOREIGN KEY ("storeId") REFERENCES "stores"("id") ON DELETE NO ACTION ON UPDATE NO ACTION
casper-processor  | query: COMMIT
casper-processor  | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'migrations'
casper-processor  | query: CREATE TABLE "migrations" ("id" SERIAL NOT NULL, "timestamp" bigint NOT NULL, "name" character varying NOT NULL, CONSTRAINT "PK_8c82d7f526340ab734260ea46be" PRIMARY KEY ("id"))
casper-processor  | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'typeorm_metadata'
casper-processor  | query: SELECT * FROM "migrations" "migrations" ORDER BY "id" DESC
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmCoreModule dependencies initialized[39m[38;5;3m +147ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mUserModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTransactionModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mStoresModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mPaymentModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:20 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mAuthModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[NestFactory] [39m[32mStarting Nest application...[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +28ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mMailerModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mMailerModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mClientsModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mHttpModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mMailerCoreModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mDiscoveryModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mAppModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mScheduleModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mConfigModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-back       | query: SELECT * FROM current_schema()
casper-back       | query: SHOW server_version;
casper-back       | query: START TRANSACTION
casper-back       | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'typeorm_metadata'
casper-back       | query: SELECT * FROM current_schema()
casper-back       | query: SELECT * FROM current_database()
casper-back       | query: SELECT "table_schema", "table_name" FROM "information_schema"."tables" WHERE ("table_schema" = 'public' AND "table_name" = 'user') OR ("table_schema" = 'public' AND "table_name" = 'transaction') OR ("table_schema" = 'public' AND "table_name" = 'payment') OR ("table_schema" = 'public' AND "table_name" = 'stores')
casper-back       | query: SELECT TRUE FROM information_schema.columns WHERE table_name = 'pg_class' and column_name = 'relispartition'
casper-back       | query: SELECT columns.*, pg_catalog.col_description(('"' || table_catalog || '"."' || table_schema || '"."' || table_name || '"')::regclass::oid, ordinal_position) AS description, ('"' || "udt_schema" || '"."' || "udt_name" || '"')::"regtype" AS "regtype", pg_catalog.format_type("col_attr"."atttypid", "col_attr"."atttypmod") AS "format_type" FROM "information_schema"."columns" LEFT JOIN "pg_catalog"."pg_attribute" AS "col_attr" ON "col_attr"."attname" = "columns"."column_name" AND "col_attr"."attrelid" = ( SELECT "cls"."oid" FROM "pg_catalog"."pg_class" AS "cls" LEFT JOIN "pg_catalog"."pg_namespace" AS "ns" ON "ns"."oid" = "cls"."relnamespace" WHERE "cls"."relname" = "columns"."table_name" AND "ns"."nspname" = "columns"."table_schema" ) WHERE ("table_schema" = 'public' AND "table_name" = 'user') OR ("table_schema" = 'public' AND "table_name" = 'transaction') OR ("table_schema" = 'public' AND "table_name" = 'stores') OR ("table_schema" = 'public' AND "table_name" = 'payment')
casper-back       | query: SELECT "ns"."nspname" AS "table_schema", "t"."relname" AS "table_name", "cnst"."conname" AS "constraint_name", pg_get_constraintdef("cnst"."oid") AS "expression", CASE "cnst"."contype" WHEN 'p' THEN 'PRIMARY' WHEN 'u' THEN 'UNIQUE' WHEN 'c' THEN 'CHECK' WHEN 'x' THEN 'EXCLUDE' END AS "constraint_type", "a"."attname" AS "column_name" FROM "pg_constraint" "cnst" INNER JOIN "pg_class" "t" ON "t"."oid" = "cnst"."conrelid" INNER JOIN "pg_namespace" "ns" ON "ns"."oid" = "cnst"."connamespace" LEFT JOIN "pg_attribute" "a" ON "a"."attrelid" = "cnst"."conrelid" AND "a"."attnum" = ANY ("cnst"."conkey") WHERE "t"."relkind" IN ('r', 'p') AND (("ns"."nspname" = 'public' AND "t"."relname" = 'user') OR ("ns"."nspname" = 'public' AND "t"."relname" = 'transaction') OR ("ns"."nspname" = 'public' AND "t"."relname" = 'stores') OR ("ns"."nspname" = 'public' AND "t"."relname" = 'payment'))
casper-back       | query: SELECT "ns"."nspname" AS "table_schema", "t"."relname" AS "table_name", "i"."relname" AS "constraint_name", "a"."attname" AS "column_name", CASE "ix"."indisunique" WHEN 't' THEN 'TRUE' ELSE'FALSE' END AS "is_unique", pg_get_expr("ix"."indpred", "ix"."indrelid") AS "condition", "types"."typname" AS "type_name" FROM "pg_class" "t" INNER JOIN "pg_index" "ix" ON "ix"."indrelid" = "t"."oid" INNER JOIN "pg_attribute" "a" ON "a"."attrelid" = "t"."oid"  AND "a"."attnum" = ANY ("ix"."indkey") INNER JOIN "pg_namespace" "ns" ON "ns"."oid" = "t"."relnamespace" INNER JOIN "pg_class" "i" ON "i"."oid" = "ix"."indexrelid" INNER JOIN "pg_type" "types" ON "types"."oid" = "a"."atttypid" LEFT JOIN "pg_constraint" "cnst" ON "cnst"."conname" = "i"."relname" WHERE "t"."relkind" IN ('r', 'p') AND "cnst"."contype" IS NULL AND (("ns"."nspname" = 'public' AND "t"."relname" = 'user') OR ("ns"."nspname" = 'public' AND "t"."relname" = 'transaction') OR ("ns"."nspname" = 'public' AND "t"."relname" = 'stores') OR ("ns"."nspname" = 'public' AND "t"."relname" = 'payment'))
casper-back       | query: SELECT "con"."conname" AS "constraint_name", "con"."nspname" AS "table_schema", "con"."relname" AS "table_name", "att2"."attname" AS "column_name", "ns"."nspname" AS "referenced_table_schema", "cl"."relname" AS "referenced_table_name", "att"."attname" AS "referenced_column_name", "con"."confdeltype" AS "on_delete", "con"."confupdtype" AS "on_update", "con"."condeferrable" AS "deferrable", "con"."condeferred" AS "deferred" FROM ( SELECT UNNEST ("con1"."conkey") AS "parent", UNNEST ("con1"."confkey") AS "child", "con1"."confrelid", "con1"."conrelid", "con1"."conname", "con1"."contype", "ns"."nspname", "cl"."relname", "con1"."condeferrable", CASE WHEN "con1"."condeferred" THEN 'INITIALLY DEFERRED' ELSE 'INITIALLY IMMEDIATE' END as condeferred, CASE "con1"."confdeltype" WHEN 'a' THEN 'NO ACTION' WHEN 'r' THEN 'RESTRICT' WHEN 'c' THEN 'CASCADE' WHEN 'n' THEN 'SET NULL' WHEN 'd' THEN 'SET DEFAULT' END as "confdeltype", CASE "con1"."confupdtype" WHEN 'a' THEN 'NO ACTION' WHEN 'r' THEN 'RESTRICT' WHEN 'c' THEN 'CASCADE' WHEN 'n' THEN 'SET NULL' WHEN 'd' THEN 'SET DEFAULT' END as "confupdtype" FROM "pg_class" "cl" INNER JOIN "pg_namespace" "ns" ON "cl"."relnamespace" = "ns"."oid" INNER JOIN "pg_constraint" "con1" ON "con1"."conrelid" = "cl"."oid" WHERE "con1"."contype" = 'f' AND (("ns"."nspname" = 'public' AND "cl"."relname" = 'user') OR ("ns"."nspname" = 'public' AND "cl"."relname" = 'transaction') OR ("ns"."nspname" = 'public' AND "cl"."relname" = 'stores') OR ("ns"."nspname" = 'public' AND "cl"."relname" = 'payment')) ) "con" INNER JOIN "pg_attribute" "att" ON "att"."attrelid" = "con"."confrelid" AND "att"."attnum" = "con"."child" INNER JOIN "pg_class" "cl" ON "cl"."oid" = "con"."confrelid"  AND "cl"."relispartition" = 'f'INNER JOIN "pg_namespace" "ns" ON "cl"."relnamespace" = "ns"."oid" INNER JOIN "pg_attribute" "att2" ON "att2"."attrelid" = "con"."conrelid" AND "att2"."attnum" = "con"."parent"
casper-back       | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'typeorm_metadata'
casper-back       | query: SELECT * FROM current_database()
casper-back       | query: SELECT * FROM current_schema()
casper-back       | query: SELECT "t".* FROM "typeorm_metadata" "t" INNER JOIN "pg_catalog"."pg_class" "c" ON "c"."relname" = "t"."name" INNER JOIN "pg_namespace" "n" ON "n"."oid" = "c"."relnamespace" AND "n"."nspname" = "t"."schema" WHERE "t"."type" IN ('VIEW', 'MATERIALIZED_VIEW') AND (1=1)
casper-back       | query: ALTER TABLE "payment" ALTER COLUMN "datetime" SET DEFAULT now()
casper-back       | query: ALTER TABLE "stores" ALTER COLUMN "blocked" SET DEFAULT false
casper-back       | query: COMMIT
casper-back       | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'migrations'
casper-back       | query: SELECT * FROM "information_schema"."tables" WHERE "table_schema" = 'public' AND "table_name" = 'typeorm_metadata'
casper-back       | query: SELECT * FROM "migrations" "migrations" ORDER BY "id" DESC
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmCoreModule dependencies initialized[39m[38;5;3m +107ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTypeOrmModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mUserModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mStoresModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mAuthModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mTransactionModule dependencies initialized[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[InstanceLoader] [39m[32mPaymentModule dependencies initialized[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mAppController {/api}:[39m[38;5;3m +309ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api, GET} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mUserController {/api/user}:[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user/block, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user/:id, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user, GET} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user/bulk, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user/:id, PATCH} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user/:id, PUT} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/user/:id, DELETE} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mAuthController {/api/auth}:[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/auth/register, POST} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/auth/verify, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/auth/login, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/auth/send-code, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/auth/reAuth, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/auth/check-code, POST} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/auth/reset-pwd, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mStoresController {/api/store}:[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/bulk, POST} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/:id, PATCH} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/:id, PUT} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/:id, DELETE} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/block, POST} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/tx/:token, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/:id, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/:id, PATCH} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/store/:id, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mPaymentController {/api/payment}:[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment, GET} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment/:id, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment/:id, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment/bulk, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment/:id, PATCH} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment/:id, PUT} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment/:id, DELETE} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mPaymentStoreController {/api/payment}:[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/payment/send-mail-bill, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mTransactionController {/api/transaction}:[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction, GET} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction/last/:id, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction/:txHash, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction/:id, GET} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction, GET} route[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction/bulk, POST} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction/:id, PATCH} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction/:id, PUT} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RouterExplorer] [39m[32mMapped {/api/transaction/:id, DELETE} route[39m[38;5;3m +0ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[RoutesResolver] [39m[32mTransactionStoreController {/api/transaction}:[39m[38;5;3m +1ms[39m
casper-back       | [32m[Nest] 32  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[NestApplication] [39m[32mNest application successfully started[39m[38;5;3m +4ms[39m
casper-processor  | [32m[Nest] 31  - [39m04/16/2022, 8:37:21 PM [32m    LOG[39m [38;5;3m[NestMicroservice] [39m[32mNest microservice successfully started[39m[38;5;3m +1205ms[39m
casper-processor  | microservice is listening

```
