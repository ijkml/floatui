---
title: Modal Dialog
category: Application
paid: true
isActive: true
ltr: {"react":{"jsxCss":[{"label":"App.jsx","code":"import { useState } from \"react\"\n\nexport default () => {\n\n    const [state, setState] = useState(true)\n\n    return (\n        state ? (\n            <div className=\"modal-text-md\">\n                <div className=\"modal-cover\" onClick={() => setState(false)}></div>\n                <div className=\"modal-container\">\n                    <div className=\"modal\">\n                        <div className=\"modal-header\">\n                            <h4>\n                                Terms and agreements\n                            </h4>\n                            <button className=\"btn-cancel\"\n                                onClick={() => setState(false)}\n                            >\n                                <svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 20 20\" fill=\"currentColor\">\n                                    <path fillRule=\"evenodd\" d=\"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\" clipRule=\"evenodd\" />\n                                </svg>\n                            </button>\n                        </div>\n                        <div className=\"modal-content\">\n                            <p>\n                                Commodo eget a et dignissim dignissim morbi vitae, mi. Mi aliquam sit ultrices enim cursus. Leo sapien, pretium duis est eu volutpat interdum eu non. Odio eget nullam elit laoreet. Libero at felis nam at orci venenatis rutrum nunc. Etiam mattis ornare pellentesque iaculis enim.\n                            </p>\n                            <p>\n                                Felis eu non in aliquam egestas placerat. Eget maecenas ornare venenatis lacus nunc, sit arcu. Nam pharetra faucibus eget facilisis pulvinar eu sapien turpis at. Nec aliquam aliquam blandit eu ipsum.\n                            </p>\n                        </div>\n                        <div className=\"modal-footer\">\n                            <button className=\"btn-primary\"\n                                onClick={() => setState(false)}\n                            >\n                                Accept\n                            </button>\n                            <button className=\"btn-secondary\"\n                                onClick={() => setState(false)}\n                            >\n                                Cancel\n                            </button>\n                        </div>\n                    </div>\n                </div>\n            </div>\n        ) : ''\n    )\n}"},{"label":"style.css","code":".modal-text-md, .modal-text-md .modal-cover {\n  top: 0px;\n  right: 0px;\n  bottom: 0px;\n  left: 0px;\n}\n\n.modal-text-md {\n  position: fixed;\n  overflow-y: auto;\n}\n.modal-text-md .modal-cover {\n  position: fixed;\n  width: 100%;\n  height: 100%;\n  background-color: #000;\n  opacity: 0.4;\n}\n.modal-text-md .modal-container {\n  display: flex;\n  align-items: center;\n  min-height: 100vh;\n  padding: 2rem 1rem 2rem 1rem;\n}\n.modal-text-md .modal-container .modal {\n  position: relative;\n  width: 100%;\n  max-width: 32rem;\n  margin-left: auto;\n  margin-right: auto;\n  background-color: #FFF;\n  border-radius: 0.375rem;\n  box-shadow: 0 10px 15px -3px #0000001a, 0 4px 6px -4px #0000001a;\n}\n.modal-text-md .modal-container .modal .modal-header {\n  display: flex;\n  align-items: center;\n  justify-content: space-between;\n  padding: 1rem;\n  border-bottom: solid 1px #e5e7eb;\n}\n.modal-text-md .modal-container .modal .modal-header h4 {\n  font-size: 1.125rem;\n  line-height: 1.75rem;\n  font-weight: 500;\n  color: #1f2937;\n}\n.modal-text-md .modal-container .modal .modal-header button {\n  padding: 0.5rem;\n  color: #9ca3af;\n  border-radius: 0.375rem;\n}\n.modal-text-md .modal-container .modal .modal-header button:hover {\n  background-color: #f3f4f6;\n}\n.modal-text-md .modal-container .modal .modal-header button svg {\n  width: 1.25rem;\n  height: 1.25rem;\n  margin-left: auto;\n  margin-right: auto;\n}\n.modal-text-md .modal-container .modal .modal-content {\n  padding: 1rem;\n  margin-top: 0.75rem;\n  font-size: 15.5px;\n  line-height: 1.625;\n  color: #6b7280;\n}\n.modal-text-md .modal-container .modal .modal-content > * + * {\n  margin-top: 0.5rem;\n}\n.modal-text-md .modal-container .modal .modal-footer {\n  margin-top: 1.25rem;\n  display: flex;\n  align-items: center;\n  gap: 0.75rem;\n  padding: 1rem;\n  border-top: solid 1px #e5e7eb;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary, .modal-text-md .modal-container .modal .modal-footer .btn-secondary {\n  padding: 0.5rem 1.5rem 0.5rem 1.5rem;\n  outline: none;\n  border-radius: 0.375rem;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary:focus, .modal-text-md .modal-container .modal .modal-footer .btn-secondary:focus {\n  box-shadow: 0 0 0 2px white, 0 0 0 4px #4f46e5;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary {\n  background-color: #4f46e5;\n  color: #FFF;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-secondary {\n  border: solid 1px #e5e7eb;\n  color: #1f2937;\n}"}],"jsxTail":[{"label":"App.jsx","code":"import { useState } from \"react\"\n\nexport default () => {\n\n    const [state, setState] = useState(true)\n\n    return (\n        state ? (\n            <div className=\"fixed inset-0 z-10 overflow-y-auto\">\n                <div className=\"fixed inset-0 w-full h-full bg-black opacity-40\" onClick={() => setState(false)}></div>\n                <div className=\"flex items-center min-h-screen px-4 py-8\">\n                    <div className=\"relative w-full max-w-lg mx-auto bg-white rounded-md shadow-lg\">\n                        <div className=\"flex items-center justify-between p-4 border-b\">\n                            <h4 className=\"text-lg font-medium text-gray-800\">\n                                Terms and agreements\n                            </h4>\n                            <button className=\"p-2 text-gray-400 rounded-md hover:bg-gray-100\"\n                                onClick={() => setState(false)}\n                            >\n                                <svg xmlns=\"http://www.w3.org/2000/svg\" className=\"w-5 h-5 mx-auto\" viewBox=\"0 0 20 20\" fill=\"currentColor\">\n                                    <path fillRule=\"evenodd\" d=\"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\" clipRule=\"evenodd\" />\n                                </svg>\n                            </button>\n                        </div>\n                        <div className=\"space-y-2 p-4 mt-3 text-[15.5px] leading-relaxed text-gray-500\">\n                            <p>\n                                Commodo eget a et dignissim dignissim morbi vitae, mi. Mi aliquam sit ultrices enim cursus. Leo sapien, pretium duis est eu volutpat interdum eu non. Odio eget nullam elit laoreet. Libero at felis nam at orci venenatis rutrum nunc. Etiam mattis ornare pellentesque iaculis enim.\n                            </p>\n                            <p>\n                                Felis eu non in aliquam egestas placerat. Eget maecenas ornare venenatis lacus nunc, sit arcu. Nam pharetra faucibus eget facilisis pulvinar eu sapien turpis at. Nec aliquam aliquam blandit eu ipsum.\n                            </p>\n                        </div>\n                        <div className=\"flex items-center gap-3 p-4 mt-5 border-t\">\n                            <button className=\"px-6 py-2 text-white bg-indigo-600 rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\"\n                                onClick={() => setState(false)}\n                            >\n                                Accept\n                            </button>\n                            <button className=\"px-6 py-2 text-gray-800 border rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\"\n                                onClick={() => setState(false)}\n                            >\n                                Cancel\n                            </button>\n                        </div>\n                    </div>\n                </div>\n            </div>\n        ) : ''\n    )\n}\n"}]},"vue":{"vueCss":[{"label":"App.vue","code":"<template>\n  <div class=\"modal-text-md\" :class=\"[open ? 'hidden' : 'block']\">\n    <div class=\"modal-cover\" :class=\"[open ? 'hidden' : 'block']\"></div>\n    <div class=\"modal-container\" :class=\"[open ? 'hidden' : 'block']\">\n      <div class=\"modal\">\n        <div class=\"modal-header\">\n          <h4>\n            Terms and agreements\n          </h4>\n          <button class=\"btn-cancel\" @click=\"modalOpen()\">\n            <svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 20 20\" fill=\"currentColor\">\n              <path fillRule=\"evenodd\"\n                d=\"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\"\n                clipRule=\"evenodd\" />\n            </svg>\n          </button>\n        </div>\n        <div class=\"modal-content\">\n          <p>\n            Commodo eget a et dignissim dignissim morbi vitae, mi. Mi aliquam sit ultrices enim cursus. Leo sapien,\n            pretium duis est eu volutpat interdum eu non. Odio eget nullam elit laoreet. Libero at felis nam at orci\n            venenatis rutrum nunc. Etiam mattis ornare pellentesque iaculis enim.\n          </p>\n          <p>\n            Felis eu non in aliquam egestas placerat. Eget maecenas ornare venenatis lacus nunc, sit arcu. Nam pharetra\n            faucibus eget facilisis pulvinar eu sapien turpis at. Nec aliquam aliquam blandit eu ipsum.\n          </p>\n        </div>\n        <div class=\"modal-footer\">\n          <button class=\"btn-primary\" @click=\"modalOpen()\">\n            Accept\n          </button>\n          <button class=\"btn-secondary\" @click=\"modalOpen()\">\n            Cancel\n          </button>\n        </div>\n      </div>\n    </div>\n  </div>\n</template>\n\n<script>\nimport { ref } from 'vue';\nexport default {\n  setup() {\n    let open = ref(false);\n    function modalOpen() {\n      open.value = !open.value;\n    }\n    return { open, modalOpen }\n  }\n}\n</script>"},{"label":"style.css","code":"  .modal-text-md, .modal-text-md .modal-cover {\n  top: 0px;\n  right: 0px;\n  bottom: 0px;\n  left: 0px;\n}\n\n.modal-text-md {\n  position: fixed;\n  overflow-y: auto;\n}\n.modal-text-md .modal-cover {\n  position: fixed;\n  width: 100%;\n  height: 100%;\n  background-color: #000;\n  opacity: 0.4;\n}\n.modal-text-md .modal-container {\n  display: flex;\n  align-items: center;\n  min-height: 100vh;\n  padding: 2rem 1rem 2rem 1rem;\n}\n.modal-text-md .modal-container .modal {\n  position: relative;\n  width: 100%;\n  max-width: 32rem;\n  margin-left: auto;\n  margin-right: auto;\n  background-color: #FFF;\n  border-radius: 0.375rem;\n  box-shadow: 0 10px 15px -3px #0000001a, 0 4px 6px -4px #0000001a;\n}\n.modal-text-md .modal-container .modal .modal-header {\n  display: flex;\n  align-items: center;\n  justify-content: space-between;\n  padding: 1rem;\n  border-bottom: solid 1px #e5e7eb;\n}\n.modal-text-md .modal-container .modal .modal-header h4 {\n  font-size: 1.125rem;\n  line-height: 1.75rem;\n  font-weight: 500;\n  color: #1f2937;\n}\n.modal-text-md .modal-container .modal .modal-header button {\n  padding: 0.5rem;\n  color: #9ca3af;\n  border-radius: 0.375rem;\n}\n.modal-text-md .modal-container .modal .modal-header button:hover {\n  background-color: #f3f4f6;\n}\n.modal-text-md .modal-container .modal .modal-header button svg {\n  width: 1.25rem;\n  height: 1.25rem;\n  margin-left: auto;\n  margin-right: auto;\n}\n.modal-text-md .modal-container .modal .modal-content {\n  padding: 1rem;\n  margin-top: 0.75rem;\n  font-size: 15.5px;\n  line-height: 1.625;\n  color: #6b7280;\n}\n.modal-text-md .modal-container .modal .modal-content > * + * {\n  margin-top: 0.5rem;\n}\n.modal-text-md .modal-container .modal .modal-footer {\n  margin-top: 1.25rem;\n  display: flex;\n  align-items: center;\n  gap: 0.75rem;\n  padding: 1rem;\n  border-top: solid 1px #e5e7eb;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary, .modal-text-md .modal-container .modal .modal-footer .btn-secondary {\n  padding: 0.5rem 1.5rem 0.5rem 1.5rem;\n  outline: none;\n  border-radius: 0.375rem;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary:focus, .modal-text-md .modal-container .modal .modal-footer .btn-secondary:focus {\n  box-shadow: 0 0 0 2px white, 0 0 0 4px #4f46e5;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary {\n  background-color: #4f46e5;\n  color: #FFF;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-secondary {\n  border: solid 1px #e5e7eb;\n  color: #1f2937;\n}\n.hidden {\n  display: none;\n}\n.block {\n  display: block;\n}"}],"vueTail":[{"code":"<template>\n  <div class=\"fixed inset-0 z-10 overflow-y-auto\">\n    <div class=\"fixed inset-0 w-full h-full bg-black opacity-40\" :class=\"[open ? 'hidden' : 'block']\"></div>\n    <div class=\"flex items-center min-h-screen px-4 py-8\" :class=\"[open ? 'hidden' : 'block']\">\n      <div class=\"relative w-full max-w-lg mx-auto bg-white rounded-md shadow-lg\">\n        <div class=\"flex items-center justify-between p-4 border-b\">\n          <h4 class=\"text-lg font-medium text-gray-800\">\n            Terms and agreements\n          </h4>\n          <button class=\"p-2 text-gray-400 rounded-md hover:bg-gray-100\" @click=\"modalOpen()\">\n            <svg xmlns=\"http://www.w3.org/2000/svg\" class=\"w-5 h-5 mx-auto\" viewBox=\"0 0 20 20\" fill=\"currentColor\">\n              <path fillRule=\"evenodd\"\n                d=\"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\"\n                clipRule=\"evenodd\" />\n            </svg>\n          </button>\n        </div>\n        <div class=\"space-y-2 p-4 mt-3 text-[15.5px] leading-relaxed text-gray-500\">\n          <p>\n            Commodo eget a et dignissim dignissim morbi vitae, mi. Mi aliquam sit ultrices enim cursus. Leo sapien,\n            pretium duis est eu volutpat interdum eu non. Odio eget nullam elit laoreet. Libero at felis nam at orci\n            venenatis rutrum nunc. Etiam mattis ornare pellentesque iaculis enim.\n          </p>\n          <p>\n            Felis eu non in aliquam egestas placerat. Eget maecenas ornare venenatis lacus nunc, sit arcu. Nam pharetra\n            faucibus eget facilisis pulvinar eu sapien turpis at. Nec aliquam aliquam blandit eu ipsum.\n          </p>\n        </div>\n        <div class=\"flex items-center gap-3 p-4 mt-5 border-t\">\n          <button @click=\"modalOpen()\"\n            class=\"px-6 py-2 text-white bg-indigo-600 rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\">\n            Accept\n          </button>\n          <button @click=\"modalOpen()\"\n            class=\"px-6 py-2 text-gray-800 border rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\">\n            Cancel\n          </button>\n        </div>\n      </div>\n    </div>\n  </div>\n</template>\n\n<script>\nimport { ref } from 'vue';\nexport default {\n  setup() {\n    let open = ref(false);\n    function modalOpen() {\n      open.value = !open.value;\n    }\n    return { open, modalOpen }\n  }\n}\n</script>","label":"App.vue"}]},"preview":"function App() {\n  const [state, setState] = useState(true);\n  useEffect(() => {\n    if (!state) setTimeout(() => setState(true), 1200);\n  }, [state]);\n  return /*#__PURE__*/React.createElement(\"div\", {\n    style: {\n      height: '580px'\n    }\n  }, state ? /*#__PURE__*/React.createElement(\"div\", {\n    className: \"fixed inset-0 z-10 overflow-y-auto\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"fixed inset-0 w-full h-full bg-black opacity-40\",\n    onClick: () => setState(false)\n  }), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"flex items-center min-h-screen px-4 py-8\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"relative w-full max-w-lg mx-auto bg-white rounded-md shadow-lg\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"flex items-center justify-between p-4 border-b\"\n  }, /*#__PURE__*/React.createElement(\"h4\", {\n    className: \"text-lg font-medium text-gray-800\"\n  }, \"Terms and agreements\"), /*#__PURE__*/React.createElement(\"button\", {\n    className: \"p-2 text-gray-400 rounded-md hover:bg-gray-100\",\n    onClick: () => setState(false)\n  }, /*#__PURE__*/React.createElement(\"svg\", {\n    xmlns: \"http://www.w3.org/2000/svg\",\n    className: \"w-5 h-5 mx-auto\",\n    viewBox: \"0 0 20 20\",\n    fill: \"currentColor\"\n  }, /*#__PURE__*/React.createElement(\"path\", {\n    fillRule: \"evenodd\",\n    d: \"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\",\n    clipRule: \"evenodd\"\n  })))), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"space-y-2 p-4 mt-3 text-[15.5px] leading-relaxed text-gray-500\"\n  }, /*#__PURE__*/React.createElement(\"p\", null, \"Commodo eget a et dignissim dignissim morbi vitae, mi. Mi aliquam sit ultrices enim cursus. Leo sapien, pretium duis est eu volutpat interdum eu non. Odio eget nullam elit laoreet. Libero at felis nam at orci venenatis rutrum nunc. Etiam mattis ornare pellentesque iaculis enim.\"), /*#__PURE__*/React.createElement(\"p\", null, \"Felis eu non in aliquam egestas placerat. Eget maecenas ornare venenatis lacus nunc, sit arcu. Nam pharetra faucibus eget facilisis pulvinar eu sapien turpis at. Nec aliquam aliquam blandit eu ipsum.\")), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"flex items-center gap-3 p-4 mt-5 border-t\"\n  }, /*#__PURE__*/React.createElement(\"button\", {\n    className: \"px-6 py-2 text-white bg-indigo-600 rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\",\n    onClick: () => setState(false)\n  }, \"Accept\"), /*#__PURE__*/React.createElement(\"button\", {\n    className: \"px-6 py-2 text-gray-800 border rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\",\n    onClick: () => setState(false)\n  }, \"Cancel\"))))) : '');\n}"}
rtl: {"react":{"jsxCss":[{"code":"import { useState } from \"react\"\n\nexport default () => {\n\n    const [state, setState] = useState(true)\n\n    return (\n        state ? (\n            <div className=\"modal-text-md\">\n                <div className=\"modal-cover\" onClick={() => setState(false)}></div>\n                <div className=\"modal-container\">\n                    <div className=\"modal\">\n                        <div className=\"modal-header\">\n                            <h4>\n                                الشروط والاتفاقيات\n                            </h4>\n                            <button className=\"btn-cancel\"\n                                onClick={() => setState(false)}\n                            >\n                                <svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 20 20\" fill=\"currentColor\">\n                                    <path fillRule=\"evenodd\" d=\"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\" clipRule=\"evenodd\" />\n                                </svg>\n                            </button>\n                        </div>\n                        <div className=\"modal-content\">\n                            <p>\n                                الألم بحد ذاته هو حب الألم، المشاكل البيئية الرئيسية، لكني أعطي هذا النوع من الوقت للتراجع، بحيث يكون هناك بعض الألم والألم العظيمين. الآن الألم يحتاج إلى سيارة، لكن الكارتون نفسه الآن. يمكنك إنشاء هذا الباب مع.\n                            </p>\n                            <p>\n                                كرة القدم ليست في شكل من أشكال الفقر. يحتاج الآن لتزيين بحيراته السامة فليكن القوس. لجعبة الحلق تحتاج إلى وسادة سهلة لكرة القدم الحكيمة القبيحة عندها. وليس شيئا لطيفا عنه.\n                            </p>\n                        </div>\n                        <div className=\"modal-footer\">\n                            <button className=\"btn-primary\"\n                                onClick={() => setState(false)}\n                            >\n                                أوافق\n                            </button>\n                            <button className=\"btn-secondary\"\n                                onClick={() => setState(false)}\n                            >\n                                تراجع\n                            </button>\n                        </div>\n                    </div>\n                </div>\n            </div>\n        ) : ''\n    )\n}","label":"App.jsx"},{"label":"style.css","code":".modal-text-md, .modal-text-md .modal-cover {\n  top: 0px;\n  right: 0px;\n  bottom: 0px;\n  left: 0px;\n}\n\n.modal-text-md {\n  position: fixed;\n  overflow-y: auto;\n}\n.modal-text-md .modal-cover {\n  position: fixed;\n  width: 100%;\n  height: 100%;\n  background-color: #000;\n  opacity: 0.4;\n}\n.modal-text-md .modal-container {\n  display: flex;\n  align-items: center;\n  min-height: 100vh;\n  padding: 2rem 1rem 2rem 1rem;\n}\n.modal-text-md .modal-container .modal {\n  position: relative;\n  width: 100%;\n  max-width: 32rem;\n  margin-left: auto;\n  margin-right: auto;\n  background-color: #FFF;\n  border-radius: 0.375rem;\n  box-shadow: 0 10px 15px -3px #0000001a, 0 4px 6px -4px #0000001a;\n}\n.modal-text-md .modal-container .modal .modal-header {\n  display: flex;\n  align-items: center;\n  justify-content: space-between;\n  padding: 1rem;\n  border-bottom: solid 1px #e5e7eb;\n}\n.modal-text-md .modal-container .modal .modal-header h4 {\n  font-size: 1.125rem;\n  line-height: 1.75rem;\n  font-weight: 500;\n  color: #1f2937;\n}\n.modal-text-md .modal-container .modal .modal-header button {\n  padding: 0.5rem;\n  color: #9ca3af;\n  border-radius: 0.375rem;\n}\n.modal-text-md .modal-container .modal .modal-header button:hover {\n  background-color: #f3f4f6;\n}\n.modal-text-md .modal-container .modal .modal-header button svg {\n  width: 1.25rem;\n  height: 1.25rem;\n  margin-left: auto;\n  margin-right: auto;\n}\n.modal-text-md .modal-container .modal .modal-content {\n  padding: 1rem;\n  margin-top: 0.75rem;\n  font-size: 15.5px;\n  line-height: 1.625;\n  color: #6b7280;\n}\n.modal-text-md .modal-container .modal .modal-content > * + * {\n  margin-top: 0.5rem;\n}\n.modal-text-md .modal-container .modal .modal-footer {\n  margin-top: 1.25rem;\n  display: flex;\n  align-items: center;\n  gap: 0.75rem;\n  padding: 1rem;\n  border-top: solid 1px #e5e7eb;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary, .modal-text-md .modal-container .modal .modal-footer .btn-secondary {\n  padding: 0.5rem 1.5rem 0.5rem 1.5rem;\n  outline: none;\n  border-radius: 0.375rem;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary:focus, .modal-text-md .modal-container .modal .modal-footer .btn-secondary:focus {\n  box-shadow: 0 0 0 2px white, 0 0 0 4px #4f46e5;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-primary {\n  background-color: #4f46e5;\n  color: #FFF;\n}\n.modal-text-md .modal-container .modal .modal-footer .btn-secondary {\n  border: solid 1px #e5e7eb;\n  color: #1f2937;\n}"}],"jsxTail":[{"label":"App.jsx","code":"import { useState } from \"react\"\n\nexport default () => {\n\n    const [state, setState] = useState(true)\n\n    return (\n        state ? (\n            <div className=\"fixed inset-0 z-10 overflow-y-auto\">\n                <div className=\"fixed inset-0 w-full h-full bg-black opacity-40\" onClick={() => setState(false)}></div>\n                <div className=\"flex items-center min-h-screen px-4 py-8\">\n                    <div className=\"relative w-full max-w-lg mx-auto bg-white rounded-md shadow-lg\">\n                        <div className=\"flex items-center justify-between p-4 border-b\">\n                            <h4 className=\"text-lg font-medium text-gray-800\">\n                                الشروط والاتفاقيات\n                            </h4>\n                            <button className=\"p-2 text-gray-400 rounded-md hover:bg-gray-100\"\n                                onClick={() => setState(false)}\n                            >\n                                <svg xmlns=\"http://www.w3.org/2000/svg\" className=\"w-5 h-5 mx-auto\" viewBox=\"0 0 20 20\" fill=\"currentColor\">\n                                    <path fillRule=\"evenodd\" d=\"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\" clipRule=\"evenodd\" />\n                                </svg>\n                            </button>\n                        </div>\n                        <div className=\"space-y-2 p-4 mt-3 text-[15.5px] leading-relaxed text-gray-500\">\n                            <p>\n                                الألم بحد ذاته هو حب الألم، المشاكل البيئية الرئيسية، لكني أعطي هذا النوع من الوقت للتراجع، بحيث يكون هناك بعض الألم والألم العظيمين. الآن الألم يحتاج إلى سيارة، لكن الكارتون نفسه الآن. يمكنك إنشاء هذا الباب مع.\n                            </p>\n                            <p>\n                                كرة القدم ليست في شكل من أشكال الفقر. يحتاج الآن لتزيين بحيراته السامة فليكن القوس. لجعبة الحلق تحتاج إلى وسادة سهلة لكرة القدم الحكيمة القبيحة عندها. وليس شيئا لطيفا عنه.\n                            </p>\n                        </div>\n                        <div className=\"flex items-center gap-3 p-4 mt-5 border-t\">\n                            <button className=\"px-6 py-2 text-white bg-indigo-600 rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\"\n                                onClick={() => setState(false)}\n                            >\n                                أوافق\n                            </button>\n                            <button className=\"px-6 py-2 text-gray-800 border rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\"\n                                onClick={() => setState(false)}\n                            >\n                                تراجع\n                            </button>\n                        </div>\n                    </div>\n                </div>\n            </div>\n        ) : ''\n    )\n}"}]},"vue":{"vueCss":[],"vueTail":[]},"preview":"function App() {\n  const [state, setState] = useState(true);\n  useEffect(() => {\n    if (!state) setTimeout(() => setState(true), 1200);\n  }, [state]);\n  return /*#__PURE__*/React.createElement(\"div\", {\n    style: {\n      height: '580px'\n    }\n  }, state ? /*#__PURE__*/React.createElement(\"div\", {\n    className: \"fixed inset-0 z-10 overflow-y-auto\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"fixed inset-0 w-full h-full bg-black opacity-40\",\n    onClick: () => setState(false)\n  }), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"flex items-center min-h-screen px-4 py-8\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"relative w-full max-w-lg mx-auto bg-white rounded-md shadow-lg\"\n  }, /*#__PURE__*/React.createElement(\"div\", {\n    className: \"flex items-center justify-between p-4 border-b\"\n  }, /*#__PURE__*/React.createElement(\"h4\", {\n    className: \"text-lg font-medium text-gray-800\"\n  }, \"\\u0627\\u0644\\u0634\\u0631\\u0648\\u0637 \\u0648\\u0627\\u0644\\u0627\\u062A\\u0641\\u0627\\u0642\\u064A\\u0627\\u062A\"), /*#__PURE__*/React.createElement(\"button\", {\n    className: \"p-2 text-gray-400 rounded-md hover:bg-gray-100\",\n    onClick: () => setState(false)\n  }, /*#__PURE__*/React.createElement(\"svg\", {\n    xmlns: \"http://www.w3.org/2000/svg\",\n    className: \"w-5 h-5 mx-auto\",\n    viewBox: \"0 0 20 20\",\n    fill: \"currentColor\"\n  }, /*#__PURE__*/React.createElement(\"path\", {\n    fillRule: \"evenodd\",\n    d: \"M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z\",\n    clipRule: \"evenodd\"\n  })))), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"space-y-2 p-4 mt-3 text-[15.5px] leading-relaxed text-gray-500\"\n  }, /*#__PURE__*/React.createElement(\"p\", null, \"\\u0627\\u0644\\u0623\\u0644\\u0645 \\u0628\\u062D\\u062F \\u0630\\u0627\\u062A\\u0647 \\u0647\\u0648 \\u062D\\u0628 \\u0627\\u0644\\u0623\\u0644\\u0645\\u060C \\u0627\\u0644\\u0645\\u0634\\u0627\\u0643\\u0644 \\u0627\\u0644\\u0628\\u064A\\u0626\\u064A\\u0629 \\u0627\\u0644\\u0631\\u0626\\u064A\\u0633\\u064A\\u0629\\u060C \\u0644\\u0643\\u0646\\u064A \\u0623\\u0639\\u0637\\u064A \\u0647\\u0630\\u0627 \\u0627\\u0644\\u0646\\u0648\\u0639 \\u0645\\u0646 \\u0627\\u0644\\u0648\\u0642\\u062A \\u0644\\u0644\\u062A\\u0631\\u0627\\u062C\\u0639\\u060C \\u0628\\u062D\\u064A\\u062B \\u064A\\u0643\\u0648\\u0646 \\u0647\\u0646\\u0627\\u0643 \\u0628\\u0639\\u0636 \\u0627\\u0644\\u0623\\u0644\\u0645 \\u0648\\u0627\\u0644\\u0623\\u0644\\u0645 \\u0627\\u0644\\u0639\\u0638\\u064A\\u0645\\u064A\\u0646. \\u0627\\u0644\\u0622\\u0646 \\u0627\\u0644\\u0623\\u0644\\u0645 \\u064A\\u062D\\u062A\\u0627\\u062C \\u0625\\u0644\\u0649 \\u0633\\u064A\\u0627\\u0631\\u0629\\u060C \\u0644\\u0643\\u0646 \\u0627\\u0644\\u0643\\u0627\\u0631\\u062A\\u0648\\u0646 \\u0646\\u0641\\u0633\\u0647 \\u0627\\u0644\\u0622\\u0646. \\u064A\\u0645\\u0643\\u0646\\u0643 \\u0625\\u0646\\u0634\\u0627\\u0621 \\u0647\\u0630\\u0627 \\u0627\\u0644\\u0628\\u0627\\u0628 \\u0645\\u0639 venenatis.                                    \"), /*#__PURE__*/React.createElement(\"p\", null, \"\\u0643\\u0631\\u0629 \\u0627\\u0644\\u0642\\u062F\\u0645 \\u0644\\u064A\\u0633\\u062A \\u0641\\u064A \\u0634\\u0643\\u0644 \\u0645\\u0646 \\u0623\\u0634\\u0643\\u0627\\u0644 \\u0627\\u0644\\u0641\\u0642\\u0631. \\u064A\\u062D\\u062A\\u0627\\u062C \\u0627\\u0644\\u0622\\u0646 \\u0644\\u062A\\u0632\\u064A\\u064A\\u0646 \\u0628\\u062D\\u064A\\u0631\\u0627\\u062A\\u0647 \\u0627\\u0644\\u0633\\u0627\\u0645\\u0629 \\u0641\\u0644\\u064A\\u0643\\u0646 \\u0627\\u0644\\u0642\\u0648\\u0633. \\u0644\\u062C\\u0639\\u0628\\u0629 \\u0627\\u0644\\u062D\\u0644\\u0642 \\u062A\\u062D\\u062A\\u0627\\u062C \\u0625\\u0644\\u0649 \\u0648\\u0633\\u0627\\u062F\\u0629 \\u0633\\u0647\\u0644\\u0629 \\u0644\\u0643\\u0631\\u0629 \\u0627\\u0644\\u0642\\u062F\\u0645 \\u0627\\u0644\\u062D\\u0643\\u064A\\u0645\\u0629 \\u0627\\u0644\\u0642\\u0628\\u064A\\u062D\\u0629 \\u0639\\u0646\\u062F\\u0647\\u0627. \\u0648\\u0644\\u064A\\u0633 \\u0634\\u064A\\u0626\\u0627 \\u0644\\u0637\\u064A\\u0641\\u0627 \\u0639\\u0646\\u0647.\")), /*#__PURE__*/React.createElement(\"div\", {\n    className: \"flex items-center gap-3 p-4 mt-5 border-t\"\n  }, /*#__PURE__*/React.createElement(\"button\", {\n    className: \"px-6 py-2 text-white bg-indigo-600 rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\",\n    onClick: () => setState(false)\n  }, \"\\u0623\\u0648\\u0627\\u0641\\u0642\"), /*#__PURE__*/React.createElement(\"button\", {\n    className: \"px-6 py-2 text-gray-800 border rounded-md outline-none ring-offset-2 ring-indigo-600 focus:ring-2\",\n    onClick: () => setState(false)\n  }, \"\\u062A\\u0631\\u0627\\u062C\\u0639\"))))) : '');\n}"}
slug: /modals
id: 3a0a185c-69f7-4911-8db7-f34e78b6c647
created_at: 3
---